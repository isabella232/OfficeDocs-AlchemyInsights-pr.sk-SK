---
title: Riešenie problémov s registráciou zariadení s Windowsom v službe Microsoft Intune
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665847"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s registráciou zariadení s Windowsom v službe Microsoft Intune

Skontrolujte zdroje uvedené nižšie a teraz vyriešte problém.
  
Niektoré bežné chybové hlásenia a kroky riešenia:
  
 **Softvér sa nedá nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula. Znova prevezmite softvérový balík pc client v konzole Intune Admin Console. Ďalšie informácie nájdete v tejto dokumentácii.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich situáciách:
  
-  Používateľ má viac zariadení zaregistrovaných ako limit zariadenia. Skontrolujte tieto dokumenty, ak [chcete odstrániť zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo zmeniť limit [zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Používatelia môžu pripojiť zariadenia Azure AD" je nastavená na "none." Nastavte ho na všetkých alebo vyberte používateľov. Ďalšie informácie nájdete v [tejto dokumentácii.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Zariadenie už zapísal iný používateľ. Ak je to tak, odstráňte zariadenie z konzoly Azure Intune alebo manuálne zrušte registráciu zariadenia pred pokusom znova.

-  Zariadenie je Windows 10 Home. Iba Windows 10 Pro, Education a Enterprise SKU sa môžu pripojiť azure Active Directory.

Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:
  
-  Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhanie registrácie. Ďalšie podrobnosti [nájdete v tomto dokumente.](https://docs.microsoft.com/intune/help-desk-operators)

-  Skontrolujte tieto dokumenty pre zoznam bežných chýb, ktoré bránia registrácii a riešenia pre každý: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a Riešenie problémov [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Zistite, ako zapísať zariadenia so systémom Windows v službe Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
