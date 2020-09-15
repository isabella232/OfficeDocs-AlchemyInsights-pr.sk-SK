---
title: Inštalácia balíka Office na terminálový server – bez platnej licencie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663132"
---
# <a name="installing-office-on-a-terminal-server"></a>Inštalácia balíka Office na terminálový Server

Nasadenie aplikácií Microsoft 365 pre podniky na serveri Windows pomocou služby Remote Desktop Services (RDS), predtým pomenovaných terminálových služieb:
  
- Musíte mať predplatné na Microsoft 365, ktoré zahŕňa aplikácie Microsoft 365 pre podniky, ako napríklad Office 365 Enterprise E3 alebo Enterprise E5. Aplikácie Microsoft 365 for Business a Microsoft 365 Apps for Business Premium nezahŕňajú aplikácie Microsoft 365 pre podniky.

- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ak chcete nainštalovať aplikácie Microsoft 365 pre podniky z RDS z centra spravovania služby Microsoft 365, v ***ktorom sa používajú predvolené nastavenia inštalácie***, postupujte podľa nasledujúcich krokov.

> [!TIP]
> Môžete si tiež stiahnuť a spustiť [nástroj Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) na inštaláciu aplikácií Microsoft 365 pre podniky v režime aktivácie zdieľaného počítača.
  
1. Skontrolujte, aké predplatné služieb Microsoft 365 máte. [Zistite, ako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ak je to potrebné, prepnite na iné predplatné na Microsoft 365. [Zistite, ako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ak je Office už nainštalovaný na serveri RDS pomocou akéhokoľvek iného predplatného služby Microsoft 365, odinštalujte ho. Ak napríklad prejdete na položku Ovládací panel, \> odinštalujte program. Ak máte problémy, odinštalujte ho pomocou [podpory spoločnosti Microsoft a Sprievodcu obnovením](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. Na serveri RDS sa prihláste do centra spravovania služby Microsoft 365 s kontom správcu a [nainštalujte si aplikácie microsoft 365 pre podniky](https://portal.office.com/OLS/MySoftware.aspx).

5. Po nainštalovaní balíka Office sa ***neotvárajte ani sa prihláste*** do žiadnej aplikácie balíka Office.

6. Na serveri RDS zapnite aktiváciu zdieľaného počítača úpravou databázy registry vykonaním týchto krokov:

1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť. Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.

2. Keď sa zobrazí výzva, vyberte možnosť Áno, ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.

3. V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je povolená Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Ďalšie podrobnosti o predpokladoch, pokyny na nastavenie a pokyny na prispôsobených inštaláciách pomocou nástroja na nasadenie balíka Office nájdete v téme [nasadenie aplikácií Microsoft 365 pre podniky pomocou služby Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Ak chcete opraviť chyby súvisiace s aktiváciou zdieľaného počítača, prečítajte si tému [Riešenie problémov s aktiváciou zdieľania počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  