---
title: Riešenie problémov s zapísať iOS zariadenia v Microsoft Intune
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507018"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať iOS zariadenia v Microsoft Intune

Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz. 
  
Niektoré bežné chybové hlásenia a kroky na vyriešenie:
  
- **Dosiahnutá krytka zariadenia** Používateľ má viac zariadení zapísaných ako limit zariadenia. Skontrolujte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Táto služba nie je podporovaná. Žiadna politika zápisu:** Služba Apple push Notification (APNS) musí byť nakonfigurovaná alebo obnovená. [V tomto dokumente](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) si prečítajte pokyny, ako to urobiť. 
    
- **Typ licencie používateľa neplatné alebo meno používateľa nie je rozpoznané:** Používateľ musí prideliť licenciu Intune alebo EMS. Skontrolujte tieto dokumenty a priraďte licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) alebo [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:
  
1. Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania. Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií. 
    
2. Prečítajte si tieto dokumenty pre zoznam bežných chýb, ktoré bránia zápisu a uznesenia pre každého: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Zistite, ako zapísať zariadenia so systémom iOS do programu Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

