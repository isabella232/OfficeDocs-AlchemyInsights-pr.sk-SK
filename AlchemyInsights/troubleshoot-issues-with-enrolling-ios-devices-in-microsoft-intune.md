---
title: Riešenie problémov s zapísať iOS zariadení Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311783"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať iOS zariadení Microsoft Intune

Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz. 
  
Niektoré bežné chybové hlásenia a rozlíšenie kroky:
  
- **Zariadenie SPP dosiahla** Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/en-us/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Táto služba nie je podporovaná. Žiadna politika Enrollment:** Apple Push oznámenia služby (APN) musí byť nakonfigurovaný alebo obnovené. Prečítať [Tento dokument](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) pre návod, ako na to. 
    
- **Používateľ licenciu typu neplatný alebo meno používateľa nebol rozpoznaný:** Užívateľ musí prideliť licenciu Windows Intune alebo EMS. Revidovať tieto dokumenty priradiť licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) alebo [Azure portál](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:
  
1. Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) pre ďalšie podrobnosti. 
    
2. Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Naučte sa registrovať iOS zariadenia Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

