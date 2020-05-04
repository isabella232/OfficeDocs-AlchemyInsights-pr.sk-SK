---
title: Inštalácia balíka Office na terminálový server-bez licencie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010629"
---
# <a name="installing-office-on-a-terminal-server"></a>Inštalácia balíka Office na terminálový Server

Nasadenie Microsoft 365 aplikácie pre podniky na Windows Server pomocou Remote Desktop Services (RDS), predtým pomenované terminálové služby:
  
- Musíte mať predplatné Microsoft 365, ktorý obsahuje Microsoft 365 aplikácie pre podniky, napríklad Office 365 Enterprise E3 alebo Enterprise E5. Microsoft 365 aplikácie pre podniky a Microsoft 365 aplikácie Business Premium plány nezahŕňajú Microsoft 365 aplikácie pre podniky.

- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ak chcete nainštalovať Microsoft 365 aplikácie pre Enterprise na RDS z Microsoft 365 admin Center, ***ktorý používa predvolené nastavenie inštalácie***, použite nasledovný postup.

> [!TIP]
> Môžete tiež stiahnuť a spustiť [Microsoft Support a zotavenie asistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 aplikácie pre podniky v režime zdieľaného počítača aktivácie.
  
1. Skontrolujte, čo Microsoft 365 predplatné máte. [Zistite, ako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ak je to potrebné, prepnite na iný Microsoft 365 predplatné. [Zistite, ako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ak Office je už nainštalovaný na serveri RDS pomocou iných Microsoft 365 predplatné, odinštalujte ho. Napríklad prechodom na Ovládací panel \> odinštalujte program. Odinštalovanie pomocou [technickej podpory spoločnosti Microsoft a obnovenie asistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak používate problémy.

4. Na serveri RDS, prihláste sa do Microsoft 365 admin Center s kontom správcu a [nainštalovať Microsoft 365 aplikácie pre podniky](https://portal.office.com/OLS/MySoftware.aspx).

5. Po nainštalovaní balíka Office, ***neotvárajte ani sa prihlásiť*** do žiadnej aplikácie balíka Office.

6. Na serveri RDS zapnúť aktiváciu zdieľaného počítača úpravou databázy Registry pomocou nasledujúcich krokov:

1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť. Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.

2. Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť Yes (Áno), čím vykonáte zmeny v zariadení.

3. V editore databázy Registry pridajte hodnotu reťazca **Sharedcomputerlicensing** s nastavením 1 podľa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je zapnutá Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Ďalšie informácie o predpoklady, pokyny na nastavenie a pokyny na prispôsobené inštalácie pomocou nástroja Office Deployment, nájdete [nasadenie Microsoft 365 aplikácie pre podniky pomocou služby vzdialenej skúsenosti s prácou s počítačom](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Ak chcete opraviť chyby súvisiace so zdieľanou aktiváciou počítača, prečítajte si článok [Riešenie problémov so zdieľanou aktiváciou počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  