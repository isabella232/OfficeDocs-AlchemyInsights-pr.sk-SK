---
title: Problémy s inštaláciou aplikácie Microsoft Defender v Macu alebo Linuxe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539695"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s inštaláciou aplikácie Microsoft Defender v Macu alebo Linuxe

**Mac**

- Pred inštaláciou balíka Microsoft Defender ATP Mac skontrolujte, či sú splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Inštalácia balíka Microsoft Defender ATP pre Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Skontrolujte informácie v súbore: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Pred inštaláciou Linuxu skontrolujte, či sú Microsoft Defender ATP splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Ako nainštalovať MDATP pre Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Ak chcete overiť, či je spustená služba MDATP, pozrite si časť [Inštalácia zlyhala.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ak chcete riešiť a riešiť problémy, ak služba nie je spustená, pozrite si tému Kroky na [riešenie problémov, ak služba MDATP nie je spustená.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Kroky na kontrolu konfigurácie klienta, overenie stavu produktu a spustenie testu zisťovania v textovom súbore systému EICAR nájdete v téme [Konfigurácia klienta.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Poznámka** Zoznam podporovaných systémov súborov pre aktivitu pri prístupe nájdete v téme [Microsoft Defender ATP pre Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)