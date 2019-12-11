---
title: Nasadenie balíka Office 365 ProPlus pre zdieľané použitie na RDS, terminálovom serveri alebo VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959474"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie balíka Office 365 ProPlus pre zdieľané použitie na RDS, terminálovom serveri alebo VDI

Nasadenie balíka Office 365 ProPlus pomocou služby vzdialenej skúsenosti s prácou s počítačom (RDS), predtým pomenované terminálové služby:
- Musíte mať Microsoft 365 pre podnikateľský plán alebo Office 365 plán, ktorý zahŕňa Office 365 ProPlus, napríklad Office 365 Enterprise E3 alebo Enterprise E5.
   > [!NOTE] 
   > Plány Office 365 Business a Office 365 Business Premium nezahŕňajú Office 365 ProPlus.
- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Môžete tiež stiahnuť a spustiť [Microsoft Support a zotavenie asistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Office 365 ProPlus v režime zdieľaného počítača aktivácie.

Ďalšie informácie o predpoklady, pokyny na nastavenie a pokyny na prispôsobené inštalácie pomocou nástroja Office Deployment nájdete [nasadenie office 365 ProPlus pomocou služby vzdialenej skúsenosti s prácou s počítačom](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Oprava chýb súvisiacich so zdieľanou aktiváciou počítača:
- Pozrite si tému [Riešenie problémov so zdieľanou aktiváciou počítača pre balík Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Pozrite si [obnovenie stavu aktivácie balíka Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Ak chcete nainštalovať Office 365 ProPlus na RDS z Microsoft 365 admin Center, ***ktorý používa predvolené nastavenie inštalácie***, použite nasledovný postup:

1.  Skontrolujte, čo Office 365 plán máte. [Prečítajte si, ako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  V prípade potreby prepnite na iný plán balíka Office 365. [Prečítajte si, ako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Ak je balík Office už nainštalovaný na serveri RDS pomocou iných plánov balíka Office 365, odinštalujte ho. Napríklad prechodom na **Ovládací panel** > **odinštalujte program**. Odinštalovanie pomocou [technickej podpory spoločnosti Microsoft a obnovenie asistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak používate problémy.
4.  Na serveri RDS, prihláste sa do Microsoft 365 admin Center s kontom správcu a [nainštalovať Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Po nainštalovaní balíka Office, ***neotvárajte ani sa prihlásiť*** do žiadnej aplikácie balíka Office.
6.  Na serveri RDS zapnúť aktiváciu zdieľaného počítača úpravou databázy Registry pomocou nasledujúcich krokov:
   1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.
   2. Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť **Yes (Áno** ), čím vykonáte zmeny v zariadení.
   3. V editore databázy Registry pridajte hodnotu reťazca **Sharedcomputerlicensing** s nastavením 1 podľa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je zapnutá Aktivácia zdieľaného počítača pre balík Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

