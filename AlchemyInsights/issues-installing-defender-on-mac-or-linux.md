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
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325264"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s inštaláciou aplikácie Microsoft Defender v Macu alebo Linuxe

**Mac**

- Pred inštaláciou aplikácie Microsoft Defender ATP pre Mac skontrolujte, či sú splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Inštalácia aplikácie Microsoft Defender ATP pre Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Skontrolujte informácie v súbore: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Pred inštaláciou aplikácie Microsoft Defender ATP pre Linux skontrolujte, či sú splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Ako nainštalovať MDATP pre Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Ak chcete overiť, či je spustená služba MDATP, pozrite si časť [Inštalácia zlyhala.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ak chcete riešiť a riešiť problémy, ak služba nie je spustená, pozrite si tému Kroky na riešenie problémov v prípade, že služba [MDATP nie je spustená.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Kroky na kontrolu konfigurácie klienta, overenie stavu produktu a spustenie testu zisťovania v textovom súbore EICAR nájdete v téme [Konfigurácia klienta.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Poznámka** Zoznam podporovaných systémov súborov pre aktivitu pri prístupe nájdete v téme [Microsoft Defender ATP pre Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)