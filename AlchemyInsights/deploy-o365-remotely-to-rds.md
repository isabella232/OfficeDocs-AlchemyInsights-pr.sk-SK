---
title: Nasadenie Microsoft 365 aplikácie pre podniky pre zdieľané použitie na RDS, Terminal Server alebo VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704720"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie Microsoft 365 aplikácie pre podniky pre zdieľané použitie na RDS, Terminal Server alebo VDI

Nasadenie Microsoft 365 aplikácie pre podniky pomocou služby vzdialenej skúsenosti s prácou s počítačom (RDS), predtým pomenované terminálové služby:
- Musíte mať Microsoft 365 pre podnikateľský plán alebo Office 365 plán, ktorý zahŕňa Microsoft 365 aplikácie pre podniky, napríklad Office 365 Enterprise E3 alebo Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 aplikácie pre podniky a Microsoft 365 Business Premium štandardné plány nezahŕňajú Microsoft 365 aplikácie pre podniky.
- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Môžete tiež stiahnuť a spustiť [Microsoft Support a zotavenie asistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 aplikácie pre podniky v režime zdieľaného počítača aktivácie.

Ďalšie informácie o predpoklady, pokyny na nastavenie a pokyny na prispôsobené inštalácie pomocou nástroja Office Deployment nájdete [nasadenie Microsoft 365 aplikácie pre podniky pomocou služby vzdialenej skúsenosti s prácou s počítačom](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Oprava chýb súvisiacich so zdieľanou aktiváciou počítača:
- Pozrite si tému [Riešenie problémov so zdieľanou aktiváciou počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Pozrite si tému [Resetovanie stavu aktivácie služby Aplikácie Microsoft 365 pre veľké organizácie](https://go.microsoft.com/fwlink/?linkid=2109218).

Ak chcete nainštalovať Microsoft 365 aplikácie pre Enterprise na RDS z Microsoft 365 admin Center, ***ktorý používa predvolené nastavenie inštalácie***, použite nasledovný postup:

1.    Skontrolujte, aké predplatné máte. [Prečítajte si, ako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    V prípade potreby prepnite na iné predplatné. [Prečítajte si, ako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Ak je balík Office už nainštalovaný na serveri RDS pomocou iných predplatených služieb spoločnosti Microsoft, odinštalujte ho. Napríklad prechodom na **Ovládací panel** > **odinštalujte program**. Odinštalovanie pomocou [technickej podpory spoločnosti Microsoft a obnovenie asistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak používate problémy.
4.    Na serveri RDS, prihláste sa do Microsoft 365 admin Center s kontom správcu a [nainštalovať Microsoft 365 aplikácie pre podniky](https://portal.office.com/OLS/MySoftware.aspx).
5.    Po nainštalovaní balíka Office, ***neotvárajte ani sa prihlásiť*** do žiadnej aplikácie balíka Office.
6.    Na serveri RDS zapnúť aktiváciu zdieľaného počítača úpravou databázy Registry pomocou nasledujúcich krokov:
   1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.
   2. Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť **Yes (Áno** ), čím vykonáte zmeny v zariadení.
   3. V editore databázy Registry pridajte hodnotu reťazca **Sharedcomputerlicensing** s nastavením 1 podľa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je zapnutá Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

