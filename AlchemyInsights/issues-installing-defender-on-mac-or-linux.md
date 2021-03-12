---
title: Problémy s inštaláciou programu Microsoft Defender v Macu alebo Linuxe
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713845"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s inštaláciou programu Microsoft Defender v Macu alebo Linuxe

**Mac**

- Pred nainštalovaním aplikácie Microsoft Defender ATP pre Mac Skontrolujte, či sú splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Inštalácia programu Microsoft Defender ATP pre Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Skontrolujte informácie v súbore: "/Library/Logs/Microsoft/mdatp/install.log".

**Linuxe**

- Pred nainštalovaním aplikácie Microsoft Defender ATP pre Linux Skontrolujte, či sú splnené systémové požiadavky. Ďalšie informácie nájdete v téme [Inštalácia programu Microsoft Defender ATP pre Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Ak chcete overiť, či je spustená služba MDATP, pozrite si tému [Inštalácia zlyhala](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Ak chcete riešiť problémy a riešiť problémy, ak nie je spustená služba, pozrite si [postup pri riešení problémov, ak nie je spustená služba mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Postup na kontrolu konfigurácie klienta, ktorý overí stav produktu, a spustite test zisťovania v textovom súbore EICAR, pozrite si tému [Konfigurácia klienta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Poznámka:** Zoznam podporovaných súborových systémov pre aktivitu v Accesse nájdete v téme [Microsoft Defender ATP pre Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).