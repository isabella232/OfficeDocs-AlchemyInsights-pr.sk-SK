---
title: Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708977"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune

Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie. 
  
Niektoré bežné chybové hlásenia a kroky na riešenie problémov:
  
- **Dosiahli ste uzáver zariadenia** Používateľ má viac zariadení zaregistrovaných ako limit zariadenia. Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Táto služba nie je podporovaná. Žiadna politika registrácie:** službu Apple push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) a postupujte podľa pokynov. 
    
- **Typ licencie používateľa je neplatný alebo sa nerozpoznalo meno používateľa:** Používateľ musí mať priradenú licenciu služby Intune alebo EMS. Pozrite si tieto dokumenty a priraďte licenciu: [centrum spravovania služieb Office](https://docs.microsoft.com/intune/licenses-assign) alebo [portál Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:
  
1. Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti. 
    
2. Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Zistite, ako zapísať zariadenia so systémom iOS do služby Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

