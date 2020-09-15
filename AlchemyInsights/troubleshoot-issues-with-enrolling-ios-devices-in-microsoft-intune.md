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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669263"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune

Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie. 
  
Niektoré bežné chybové hlásenia a kroky na riešenie problémov:
  
- **Dosiahli ste uzáver zariadenia** Používateľ má viac zariadení zaregistrovaných ako limit zariadenia. Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Táto služba nie je podporovaná. Žiadna politika registrácie:** službu Apple push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) a postupujte podľa pokynov. 
    
- **Typ licencie používateľa je neplatný alebo sa nerozpoznalo meno používateľa:** Používateľ musí mať priradenú licenciu služby Intune alebo EMS. Pozrite si tieto dokumenty a priraďte licenciu: [centrum spravovania služieb Office](https://docs.microsoft.com/intune/licenses-assign) alebo [portál Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:
  
1. Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti. 
    
2. Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Zistite, ako zapísať zariadenia so systémom iOS do služby Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

