---
title: Riešenie problémov s zapísať iOS zariadení Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507018"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať iOS zariadení Microsoft Intune

Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz. 
  
Niektoré bežné chybové hlásenia a rozlíšenie kroky:
  
- **Zariadenie SPP dosiahla** Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Táto služba nie je podporovaná. Žiadna politika Enrollment:** Apple Push oznámenia služby (APN) musí byť nakonfigurovaný alebo obnovené. Prečítať [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pre návod, ako na to. 
    
- **Používateľ licenciu typu neplatný alebo meno používateľa nebol rozpoznaný:** Užívateľ musí prideliť licenciu Windows Intune alebo EMS. Revidovať tieto dokumenty priradiť licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) alebo [Azure portál](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:
  
1. Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti. 
    
2. Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Naučte sa registrovať iOS zariadenia Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

