---
title: 'Skener AIP: inštalácia a konfigurácia'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934272"
---
# <a name="aip-scanner-installation-and-configuration"></a>Skener AIP: inštalácia a konfigurácia

**Ak chcete nainštalovať skener AIP, postupujte podľa odporúčaných pokynov:**

1. Ak vykonávate inováciu a nevykonáte čistú inštaláciu, skontrolujte, či ste postupovali podľa pokynov na inováciu skenera [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pre jednotného klienta označenia, pozrite si inovovanie skenera Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Overte, či spĺňate všetky [požiadavky na nastavenia brány firewall a sieťovej infraštruktúry.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Skontrolujte, či [sú politiky nastavené na](https://docs.microsoft.com/azure/information-protection/configure-policy) automatické označovanie alebo majú v politike predvolené označenie.
4. Presvedčte sa, že príslušný typ súboru je nakonfigurovaný na označenie alebo ochranu podľa popisu v časti Typy súborov podporované klientom [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Okrem toho, ak chcete zmeniť predvolené správanie, postupujte podľa týchto pokynov: [Zmena predvolenej úrovne ochrany súborov](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Overte, či používateľské konto nakonfigurované na spustenie služby skenera má povolenia na prístup ku všetkým nakonfigurovaným odklada priestorom.
6. Ak problémy pretrváva, exportujte denníky skenerov a pridajte ich do lístka technickej podpory.

**Exportovanie denníkov skenera informácií Azure**

1. V kontexte používateľa služby skenera prejdite na položku %localappdata%\Microsoft\MSIP.
2. Komprimujte celý obsah pod priečinok MSIP.
3. Uložte denníky podľa vášho výberu a priložte ich k žiadosti o službu.
4. Môžete tiež použiť [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Ďalšie informácie nájdete v téme:**
- [Nasadenie skenera Azure Information Protection na automatické klasifikáciu a ochranu súborov](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Zadanie a použitie parametra Token pre Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Spustenie cyklu zisťovania a zobrazenie zostáv pre skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Kontrola dokumentácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Požiadavky na službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Stiahnutie klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
