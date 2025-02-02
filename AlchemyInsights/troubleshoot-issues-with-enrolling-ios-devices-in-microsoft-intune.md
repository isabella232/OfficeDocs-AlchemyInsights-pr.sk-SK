---
title: Riešenie problémov s zaregistrovaním zariadení so systémom iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047991"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení so systémom iOS v Microsoft Intune

Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie. 
  
Niektoré bežné chybové hlásenia a kroky na riešenie tohto problémov:
  
- **Dosiahol sa kryt zariadenia** Používateľ má zaregistrovaných viac zariadení, ako je limit zariadení. Skontrolujte tieto dokumenty a [odstráňte zariadenie alebo](https://docs.microsoft.com/intune/devices-wipe) zmeňte limit [zariadení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Táto služba nie je podporovaná. Žiadna politika registrácie: Službu** spoločnosti Apple Push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť. V [tomto dokumente](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) nájdete pokyny, ako to urobiť. 
    
- **Typ používateľskej licencie Neplatný alebo Meno používateľa sa nerozpoznalo:** Používateľovi je potrebné priradiť licenciu na Intune alebo EMS. Pozrite si tieto dokumenty a priraďte licenciu prostredníctvom: [Office spravovania alebo](https://docs.microsoft.com/intune/licenses-assign) [portálu Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Ďalšie zdroje informácií na vyriešenie problému:
  
1. Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie. Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente. 
    
2. V týchto dokumentoch nájdete zoznam bežných chýb, ktoré v každej z nich bránia registrácii a riešeniam: Príručka na [riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a Riešenie problémov [s dokumentom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Zistite, ako zaregistrovať zariadenia so systémom iOS vo Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

