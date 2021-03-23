---
title: Zobrazuje sa mi zablokované podmieneným prístupom s kompatibilným zariadením
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037076"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Zobrazuje sa mi zablokované podmieneným prístupom s kompatibilným zariadením

**Veľmi odporúčaná nástroje**

- [Nástroj na riešenie problémov s registráciou zariadenia](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – komplexný nástroj, ktorý pomáha riešiť najbežnejšie problémy s registráciou zariadenia.
- [Test pripojenia k registrácii zariadenia](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – nástroj používaný na zabezpečenie toho, že zariadenie môže získať prístup ku koncovým bodom registrácie zariadenia pod systémovým kontom.
- [Skript čistenia zariadenia Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – nástroj, ktorý sa používa na vyhľadanie a spravovanie zastaraných zariadení vo vašom prostredí.

Tu je niekoľko bežných dôvodov, prečo podmienený prístup môže zlyhať v prípade vyhovujúceho zariadenia alebo dôvody, prečo sa používateľom môže stať, že sa v **tejto správe nedostanete** do organizačného zdroja.

1. **Zariadenie sa nenachádza v požadovanom stave zariadenia s MDM**:

Overte, či je zariadenie zaregistrované so schváleným poskytovateľom MDM, ako je napríklad Intune, a *označené ako vyhovujúce*. Ďalšie informácie o službe Intune nájdete v tomto [dokumente](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Ak chcete lepšie pochopiť súlad s požiadavkami a službou Intune, pozrite si tému [Použitie politiky dodržiavania súladu na nastavenie pravidiel pre zariadenia, ktoré spravujete so](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)službou Intune. Ak máte problémy s zaregistrovaním zariadenia so službou Intune, vyhľadajte Podrobnosti o riešení problémov pri [riešení problémov s prihlásením zariadenia v Microsofte](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Ak chcete pokračovať v podpore služby Intune, Vytvorte žiadosť o technickú podporu. Ak to chcete urobiť, navštívte [stránku pomoc a technická podpora služby Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Zariadenie nie je pripojené k sieti organizácie**:

Ak chcete získať prístup k organizačným zdrojom, zariadenie musí byť pripojené k sieti organizácie, a to buď prostredníctvom priameho pripojenia alebo virtuálnej súkromnej siete (VPN), a tiež pripojené k lokálnemu alebo službe Azure Active Directory. Ak sa chcete k pracovnému zariadeniu zapojiť do siete organizácie, pozrite si tému [pripojenie k pracovnému zariadeniu k sieti vašej organizácie](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Ak chcete zaregistrovať osobné alebo BYOD zariadenie, pozrite si tému [registrácia osobného zariadenia v sieti vašej organizácie](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Ak chcete overiť, či sa zariadenie pripojilo k sieti, môžete postupovať podľa krokov uvedených v téme registrované zariadenia [tu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) alebo pracovné zariadenia [tu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Ak chcete vyriešiť problém s pripojením k sieti org, postupujte podľa nižšie uvedených pokynov:

    1. Prihláste sa do Windowsu pomocou svojho pracovného alebo školského konta, napríklad alain@contoso.com.
    2. Pripojte sa k sieti vašej organizácie prostredníctvom siete VPN alebo funkcie DirectAccess.
    3. Po pripojení stlačte kláves s **logom Windows + L** , čím uzamknete zariadenie.
    4. Odomknutie zariadenia pomocou pracovného alebo školského konta a potom skúste znova získať prístup k problematickej aplikácii alebo službe.

Ak sa vám zobrazí chybové hlásenie o tom, že sa **tu nedá** Zobraziť, problém je pravdepodobne inde.

3. **Operačný systém nie je podporovaný**:

Uistite sa, že používate podporovanú verziu operačného systému vrátane týchto:

- **Klient systému Windows**: Windows 7 alebo novšia verzia

- **Windows Server**: windows Server 2008 R2 alebo novšia verzia

- **MacOS**: MacOS X alebo novšia verzia

- **Android a iOS**: Najnovšia verzia operačných systémov Android a iOS pre mobilné zariadenia

4. **Webový prehliadač nie je podporovaný**:

Nižšie nájdete podporované prehliadače. Pre podporu prehliadača Chrome s Windowsom 1703 alebo novšími verziami sa vyžaduje rozšírenie kont Windowsu 10. Pre Edge 85 + musí byť používateľ prihlásený na správne odovzdanie informácií o zhode zariadenia. Ďalšie informácie nájdete [tu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Windows Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: spravovaný prehliadač Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Ďalšie informácie nájdete v [téme tu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)sa **nedá zobraziť** hlásenie a kroky na riešenie problémov.
