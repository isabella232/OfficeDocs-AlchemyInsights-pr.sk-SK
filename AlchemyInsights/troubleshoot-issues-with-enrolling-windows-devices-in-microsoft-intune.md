---
title: Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311580"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune

Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz. 
  
Niektoré bežné chybové hlásenia a rozlíšenie kroky:
  
 **Nemôže byť nainštalovaný softvér, 0x80cf4017:** Váš účet certifikátu skončila. Re-Stiahnuť softvérový balík PC klienta v Intune Admin konzole. Ďalšie informácie v tejto dokumentácii. 
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch: 
  
1. Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/en-us/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Používatelia môžu pripojiť zariadenia Azure AD" je nastavený na "none". Nastavte ju na všetky, alebo vybrať používateľov. Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) ďalšie informácie. 
    
3. Zariadenie je už zaregistrovaná iným používateľom. Ak je to prípad, odstrániť zariadenie z Azure Intune konzoly alebo manuálne unenroll zariadenie pred opätovným pokusom.
    
4. Zariadenie je Windows 10 Home. Iba Windows 10 Pro, vzdelávanie a Enterprise SKU môžete pripojiť Azure služby Active Directory.
    
Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:
  
1. Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) pre ďalšie podrobnosti. 
    
2. Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Naučte sa zapísať zariadenia so systémom Windows v spoločnosti Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

