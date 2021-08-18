---
title: Nasadenie Aplikácie Microsoft 365 pre veľké organizácie na zdieľané používanie v RDS, terminálovom serveri alebo VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325618"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie Aplikácie Microsoft 365 pre veľké organizácie na zdieľané používanie v RDS, terminálovom serveri alebo VDI

Na nasadenie Aplikácie Microsoft 365 pre veľké organizácie pomocou služieb vzdialenej pracovnej plochy (RDS), predtým s názvom Terminálové služby:

- Musíte mať plán služby Microsoft 365 For Business alebo plán Office 365, ktorý zahŕňa Aplikácie Microsoft 365 pre veľké organizácie, napríklad Office 365 Enterprise E3 alebo Enterprise E5.
   **Poznámka:** Aplikácie Microsoft 365 pre podnikateľov plány Microsoft 365 Business Standard plány nezahŕňajú Aplikácie Microsoft 365 pre veľké organizácie.
- Aktiváciu [zdieľaného počítača je potrebné zapnúť.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Poznámka:** Aplikáciu Microsoft Office si môžete stiahnuť a spustiť [Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Aplikácie Microsoft 365 pre veľké organizácie v režime aktivácie zdieľaného počítača.

Ďalšie informácie o predpokladoch, pokynoch na nastavenie a návodoch na prispôsobenie inštalácií pomocou nástroja na nasadenie balíka Office nájdete v téme Nasadenie Aplikácie Microsoft 365 pre veľké organizácie pomocou služieb vzdialenej [pracovnej plochy.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Oprava chýb súvisiacich s aktiváciou zdieľaného počítača:

- Pozrite [si tému Riešenie problémov s aktiváciou zdieľaného počítača pre Aplikácie Microsoft 365 pre veľké organizácie.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Pozrite si tému [Resetovanie stavu aktivácie služby Aplikácie Microsoft 365 pre veľké organizácie](https://go.microsoft.com/fwlink/?linkid=2109218).

Ak chcete nainštalovať inštaláciu Aplikácie Microsoft 365 pre veľké organizácie rds z aplikácie Centrum spravovania služby Microsoft 365, ***ktorá používa predvolené*** nastavenia inštalácie, postupujte takto:

1. Skontrolujte, aké predplatné máte. [Zistite, ako na to.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. V prípade potreby prejdite na iné predplatné. [Zistite, ako na to.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Ak Office nainštalovaný na serveri RDS pomocou iných predplatných od spoločnosti Microsoft, odinštalujte ho. Napríklad, ak v ovládacom paneli  >  **odinštalujete program.** Ak sa [u vás Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) odinštalujte ho pomocou služby Microsoft Support and Recovery Assistant.
4. Na serveri RDS sa prihláste do aplikácie Centrum spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte Aplikácie Microsoft 365 pre veľké organizácie](https://portal.office.com/OLS/MySoftware.aspx).
5. Po Office aplikácie ***neotvorte žiadne aplikácie balíka Office ani*** sa do Office prihlásiť.
6. Na serveri RDS povoľte aktiváciu zdieľaného počítača úpravou databázy Registry pomocou týchto krokov:
   1. Kliknite pravým tlačidlom Windows tlačidlo ľavej dolnej časti obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte príkaz **regedit** a potom vyberte tlačidlo **OK.**
   2. Keď sa **zobrazí** výzva, aby ste editoru databázy Registry umožnili vykonávať zmeny v zariadení, vyberte možnosť Áno.
   3. V Editore databázy Registry pridajte hodnotu **reťazca SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveri RDS sa ***prihláste ako koncový používateľ a overte,*** či je aktivácia zdieľaného počítača [zapnutá Aplikácie Microsoft 365 pre veľké organizácie.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
