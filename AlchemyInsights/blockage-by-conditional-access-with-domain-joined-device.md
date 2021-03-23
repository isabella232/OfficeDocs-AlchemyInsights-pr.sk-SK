---
title: Zobrazuje sa mi blokovanie podmieneným prístupom k zariadeniam pripojenému k doméne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038102"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Zobrazuje sa mi blokovanie podmieneným prístupom k zariadeniam pripojenému k doméne

**Veľmi odporúčaná nástroje**

[Nástroj na riešenie problémov s registráciou zariadenia](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – nástroj, ktorý pomáha pri riešení bežných problémov s registráciou zariadenia.

[Otestujte skript pripojenia k registrácii zariadenia](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, ktorý pomáha zabezpečiť, že zariadenie môže získať prístup ku koncovým bodom registrácie zariadenia pod systémovým kontom.

[Skript čistenia zariadenia Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, ktorý umožňuje vyhľadávať a spravovať zastarané zariadenia vo vašom prostredí.

Tu je niekoľko bežných dôvodov, prečo podmienený prístup môže zlyhať v zariadení, ktoré sa pripojilo k doméne (hybridná Azure AD).

1. **V zariadení nie je k dispozícii žiadne služby Azure AD PRT** – je potrebné zabezpečiť, aby zariadenie vytvorilo token primárneho obnovenia Azure AD (PRT). Ďalšie informácie o PRT nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Ak chcete overiť, či máte službu Azure AD PRT, môžete spustiť `dsregcmd/status` príkaz v zariadení a overiť, či sa "AzureAdPrt" rovná "Yes" (Áno).

Ak je argument "AzureAdPrt" "nie", skontrolujte nasledovné:

- **Či máte externé prostredie so službou AD FS a nie je dosiahnuteľné od domácich sietí používateľov**: v tomto prípade skontrolujte, či sú koncové body "usernamemixed" prístupné z extranetu. Ak sa vaša AD FS nachádza za VPN, zabezpečte, aby sa používatelia pripojili k sieti VPN a opätovne sa prihlásili do zariadenia. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Či je modul TPM zariadenia chybný, a preto nedokáže overiť zariadenie**: začiarknite políčko TPM. msc a zistite, či je stav modulu TPM pripravený. Ak to tak nie je, spustite `dsregcmd/leave` a nechajte zariadenie opätovne pripájať sa k službe Azure AD. Potom skúste to znova. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- Používate **poskytovateľa identity tretej strany, ktorý nepodporuje WS-Trust protokol**. Ako je popísané v našich dokumentoch, hybridné Azure AD-pripojené zariadenia nemôžu v tomto prípade fungovať. Ak máte pomoc, obráťte sa na svojho poskytovateľa identity.

2. **Používatelia používajú prehliadač Chrome bez kont Windowsu 10** alebo **Office Extension Chrome automaticky nepoužíva PRT v zariadeniach s funkciou AAD alebo hybridné AAD**: to vedie k zlyhaniu všetkých politík podmieneného prístupu založených na zariadení, pričom sa zobrazí chybové hlásenie neregistrované zariadenie. Ak chcete používať prehliadač Chrome správne, musíte nainštalovať konto Windows 10 alebo rozšírenie balíka Office do prehliadača Chrome používateľov cez SCCM alebo Intune. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Ak nie je možné rozšíriť rozšírenie na diaľku, upozorniť používateľov na manuálnu inštaláciu niektorej z vyššie uvedených rozšírení na prístup k aplikáciám za podmieneným prístupom založeným na zariadení. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Zariadenie bolo správne pripojené k hybridnej službe Azure AD, ale bolo neúmyselne odstránené alebo vypnuté, a to buď z dôvodu zmeny synchronizácie v službe Azure AD Connect alebo na portáli Azure**: Ak sa to stane, objekt zariadenia sa už nerozpoznal ako úplne pripojené zariadenie, hoci stav "AzureAdJoined" a "PRT" sa v zariadení zobrazuje ako platný.

Ak chcete tento problém vyriešiť, spustite `dsregcmd/leave` príslušné zariadenia a nechajte ich opätovne spojiť so službou Azure AD. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Ak sú vaše zariadenia vo Windowse 10, 1809 Update, so serverom VPN/cloud proxy a pozrite si tému problémy so stavom "AzureAdPrt" alebo akoukoľvek aplikáciou s problémom SSO (Outlook sa nepripája k poštovej schránke, aj keď ste mali PRT), uistite sa, že máte tento patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) alebo Kumulatívna aktualizácia [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , aby sa zabránilo zlyhaniu PRT na týchto strojoch.

















