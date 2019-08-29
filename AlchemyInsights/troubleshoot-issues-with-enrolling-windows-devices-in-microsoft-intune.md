---
title: Riešenie problémov s zapísať Windows zariadenia v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665847"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať Windows zariadenia v Microsoft Intune

Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz.
  
Niektoré bežné chybové hlásenia a kroky na vyriešenie:
  
 **Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu vášho konta uplynula. Re-download PC client softvérový balík v konzole Intune admin. Prečítajte si túto dokumentáciu pre viac informácií.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:
  
-  Používateľ má viac zariadení zapísaných ako limit zariadenia. Skontrolujte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Používatelia môžu pripojiť zariadenia k Azure AD" je nastavená na "none." Nastavte ho na možnosť všetky alebo vyberte používateľov. Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pre viac informácií.

-  Zariadenie je už zapísané iným používateľom. Ak je tomu tak, odstráňte zariadenie z konzoly Azure Intune alebo manuálne zrušte registráciu zariadenia pred pokusom znova.

-  Zariadenie je Windows 10 Home. Azure Active Directory sa môže pripojiť iba Windows 10 Pro, vzdelávanie a Enterprise SKUs.

Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:
  
-  Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania. Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií.

-  Prečítajte si tieto dokumenty pre zoznam bežných chýb, ktoré bránia zápisu a uznesenia pre každého: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Naučte sa, ako zapísať zariadenia Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
