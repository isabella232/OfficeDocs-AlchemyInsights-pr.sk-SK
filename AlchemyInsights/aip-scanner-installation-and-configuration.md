---
title: 'AIP Scanner: Inštalácia a konfigurácia'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358564"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP Scanner: Inštalácia a konfigurácia

**Ak chcete nainštalovať skener AIP, postupujte podľa odporúčaných pokynov**:

1. Ak vykonávate inováciu a nevykonávate čistú inštaláciu, uistite sa, že ste postupovali v pokynoch na [inováciu skenera Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pre klienta zjednoteného označovania, pozrite si [Aktualizácia skenera Azure Information Protection Scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Overte, či ste v súlade so všetkými [požiadavkami na nastavenie brány firewall a sieťovej infraštruktúry](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Uistite sa, že vaše [politiky sú nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatické označovanie alebo majú predvolenú menovku v politike.
4. Uistite sa, že príslušný typ súboru je nakonfigurovaný na označenie/ochrana, ako je popísané v [typy súborov podporovaných Azure informácie ochrana klienta](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Okrem toho, ak chcete zmeniť predvolené správanie, postupujte podľa týchto pokynov: [Zmena predvolenej úrovne ochrany súborov](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Overte, či používateľské konto nakonfigurované na spustenie služby skener má povolenia na prístup ku všetkým nakonfigurovaným úložiskách.
6. Ak sa problémy stále vyskytnú, exportujte denníky skenera a pridajte ich do svojho lístka podpory.

**Exportovať denníky Azure informácie ochrany skenera**

1. Prejdite na%localappdata%\Microsoft\MSIP v kontexte používateľa so službou skener.
2. ZIP všetok obsah v priečinku MSIP.
3. Uložte protokoly podľa vášho výberu polohy a priložte ich k požiadavke na službu.
4. Môžete tiež použiť [export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Ďalšie informácie nájdete v téme**:
- [Nasadenie Azure Information Protection Scanner automaticky klasifikovať a chrániť súbory](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Zadajte a použite token parameter pre overovanie set-AIP](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Spustenie cyklu zisťovania a zobrazenie zostáv pre skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Preskúmanie Azure informácie o ochrane dokumentácie](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Požiadavky na Azure informácie o ochrane](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Stiahnuť Azure informácie o ochrane klienta](https://www.microsoft.com/download/details.aspx?id=53018)
