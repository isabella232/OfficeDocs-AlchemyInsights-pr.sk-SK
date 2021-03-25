---
title: Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané používanie v RDS, terminálovom serveri alebo VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200688"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané používanie v RDS, terminálovom serveri alebo VDI

Nasadenie aplikácií Microsoft 365 pre podniky pomocou služieb Remote Desktop Services (RDS), predtým pomenovaných terminálových služieb:

- Musíte mať plán služieb Microsoft 365 for Business alebo plán Office 365, ktorý zahŕňa aplikácie Microsoft 365 pre podniky, ako napríklad Office 365 Enterprise E3 alebo Enterprise E5.
   > [!NOTE]
   > Microsoft 365 Apps for Business a Microsoft 365 Business Standard plány nezahŕňajú aplikácie Microsoft 365 pre podniky.
- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Môžete si tiež stiahnuť a spustiť [nástroj Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) na inštaláciu aplikácií Microsoft 365 pre podniky v režime aktivácie zdieľaného počítača.

Ďalšie informácie o predpokladoch, pokyny na nastavenie a pokyny týkajúce sa prispôsobených inštalácií pomocou nástroja na nasadenie balíka Office nájdete v téme [nasadenie aplikácií Microsoft 365 pre podniky pomocou služby Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Riešenie chýb súvisiacich s aktiváciou zdieľaného počítača:

- Pozrite si tému [Riešenie problémov s aktiváciou zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pozrite si tému [Resetovanie stavu aktivácie služby Aplikácie Microsoft 365 pre veľké organizácie](https://go.microsoft.com/fwlink/?linkid=2109218).

Ak chcete nainštalovať aplikácie Microsoft 365 pre podniky z RDS z centra spravovania služby Microsoft 365, v ***ktorom sa používajú predvolené nastavenia inštalácie***, postupujte takto:

1. Skontrolujte, aké predplatné máte. [Zistite, ako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)na to.
2. Ak je to potrebné, prepnite na iné predplatné. [Zistite, ako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)na to.
3. Ak je balík Office už nainštalovaný na serveri RDS pomocou iného predplatného služby Microsoft, odinštalujte ho. Ak napríklad prejdete na položku **Ovládací panel**,  >  **odinštalujte program**. Ak máte problémy, odinštalujte ho pomocou [podpory spoločnosti Microsoft a Sprievodcu obnovením](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4. Na serveri RDS sa prihláste do centra spravovania služby Microsoft 365 s kontom správcu a [nainštalujte si aplikácie microsoft 365 pre podniky](https://portal.office.com/OLS/MySoftware.aspx).
5. Po nainštalovaní balíka Office sa ***neotvárajte ani sa prihláste*** do žiadnej aplikácie balíka Office.
6. Na serveri RDS zapnite aktiváciu zdieľaného počítača úpravou databázy registry vykonaním týchto krokov:
   1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte **príkaz regedit** a potom kliknite na **tlačidlo OK**.
   2. Keď sa zobrazí výzva, vyberte možnosť **Áno** , ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.
   3. V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je povolená Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
