---
title: Riešenie problémov s zaregistrovaním Windows zariadení v Microsoft Intune
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
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981056"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním Windows zariadení v Microsoft Intune

Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.
  
Niektoré bežné chybové hlásenia a kroky na riešenie tohto problémov:
  
 **Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula. Znova si stiahnite softvérový balík PC Client v správcovskej konzole služby Intune. Ďalšie informácie nájdete v tejto dokumentácii.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich scenároch:
  
-  Používateľ má zaregistrovaných viac zariadení, ako je limit zariadení. Skontrolujte tieto dokumenty a [odstráňte zariadenie alebo](https://docs.microsoft.com/intune/devices-wipe) zmeňte limit [zariadení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Možnosť Používatelia môžu pripojiť zariadenia k službe Azure AD je nastavená na možnosť žiadne. Nastavte ho všetkým alebo vyberte používateľov. Ďalšie [informácie nájdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) tejto dokumentácii.

-  Zariadenie už zaregistroval iný používateľ. V takom prípade zariadenie odstráňte z konzoly služby Azure Intune alebo pred zopakovaním pokusu manuálne zariadenie znova zaregistrujte.

-  Zariadenie je Windows 10 Home. K Windows 10 Pro pripojiť sa môžu len SKU SKU, education a enterprise Azure Active Directory.

Ďalšie zdroje informácií na vyriešenie problému:
  
-  Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie. Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.

-  V týchto dokumentoch nájdete zoznam bežných chýb, ktoré v každej z nich bránia registrácii a riešeniam: Príručka na [riešenie problémov](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a Riešenie problémov [s dokumentom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Zistite, ako zaregistrovať Windows zariadenia v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
