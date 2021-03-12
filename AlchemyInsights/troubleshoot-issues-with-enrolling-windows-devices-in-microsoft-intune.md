---
title: Riešenie problémov s zaregistrovaním zariadení s Windowsom v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708905"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení s Windowsom v službe Microsoft Intune

Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.
  
Niektoré bežné chybové hlásenia a kroky na riešenie problémov:
  
 **Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula. Opätovné stiahnutie balíka klientskeho softvéru PC v konzole správcu služby Intune. Ďalšie informácie nájdete v tejto dokumentácii.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich prípadoch:
  
-  Používateľ má viac zariadení zaregistrovaných ako limit zariadenia. Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Používatelia sa môžu pripájať k zariadeniam Azure AD" je nastavená na hodnotu "none" (žiadne). Nastavte ju na možnosť všetci alebo vyberte položku Používatelia. Ďalšie informácie nájdete v [tejto dokumentácii](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Zariadenie je už zaregistrované iným používateľom. Ak ide o tento prípad, odstráňte zariadenie zo služby Azure Intune Console alebo manuálne zrušte registráciu zariadenia pred opätovným pokusom.

-  Zariadenie je Windows 10 Home. K službe Azure Active Directory sa môžu pridať len Windows 10 Pro, Education a Enterprise SKU.

Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:
  
-  Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.

-  Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Zistite, ako sa prihlásiť do zariadení s Windowsom v službe Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
