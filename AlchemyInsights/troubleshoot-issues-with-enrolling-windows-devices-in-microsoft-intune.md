---
title: Riešenie problémov s zaregistrovaním zariadení s Windowsom v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808986"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení s Windowsom v Microsoft Intune

Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.
  
Niektoré bežné chybové hlásenia a kroky na riešenie tohto problémov:
  
 **Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula. Znova si stiahnite softvérový balík PC Client v správcovskej konzole služby Intune. Ďalšie informácie nájdete v tejto dokumentácii.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich scenároch:
  
-  Používateľ má zaregistrovaných viac zariadení, ako je limit zariadení. Skontrolujte tieto dokumenty a [odstráňte zariadenie alebo](https://docs.microsoft.com/intune/devices-wipe) zmeňte limit [zariadení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Možnosť Používatelia môžu pripojiť zariadenia k službe Azure AD je nastavená na možnosť žiadne. Nastavte ho všetkým alebo vyberte používateľov. Ďalšie [informácie nájdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) tejto dokumentácii.

-  Zariadenie už zaregistroval iný používateľ. V takom prípade zariadenie odstráňte z konzoly služby Azure Intune alebo pred zopakovaním pokusu manuálne zariadenie znova zaregistrujte.

-  Zariadenie je Windows 10 Home. Do služby Azure Active Directory sa môžu pripojiť iba SKU Windowsu 10 Pro, Education a Enterprise.

Ďalšie zdroje informácií na vyriešenie problému:
  
-  Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie. Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.

-  V týchto dokumentoch nájdete zoznam bežných chýb, ktoré v každej z nich bránia registrácii a riešeniam: Príručka na [riešenie problémov](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a Riešenie problémov [s dokumentom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Zistite, ako zaregistrovať zariadenia s Windowsom v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
