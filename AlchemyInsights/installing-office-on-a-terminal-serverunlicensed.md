---
title: Inštalácia balíka Office na terminálový Server - bez licencie
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508643"
---
# <a name="installing-office-on-a-terminal-server"></a>Inštalácia balíka Office na terminálový Server

Nasadenie aplikácií Microsoft 365 pre podniky na serveri Windows Server pomocou služieb vzdialenej skúsenosti s prácou s počítačom (RDS), predtým s názvom Terminálové služby:
  
- Musíte mať predplatné na Microsoft 365, ktoré zahŕňa aplikácie Microsoft 365 pre podniky, napríklad Office 365 Enterprise E3 alebo Enterprise E5. Plány Microsoft 365 Apps for business a Microsoft 365 Apps for business Premium nezahŕňajú aplikácie Microsoft 365 pre podniky.

- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ak chcete nainštalovať Microsoft 365 Aplikácie pre podniky na RDS z Centra spravovania Služby Microsoft 365, ***ktorý používa predvolené nastavenia inštalácie***, postupujte nasledovne.

> [!TIP]
> Môžete tiež prevziať a spustiť [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 Apps pre podniky v režime aktivácie zdieľaného počítača.
  
1. Skontrolujte, aké predplatné na Microsoft 365 máte. [Prečítajte si, ako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. V prípade potreby prepnite na iné predplatné služby Microsoft 365. [Prečítajte si, ako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ak je balík Office už nainštalovaný na serveri RDS pomocou iných predplatných služieb Microsoft 365, odinštalujte ho. Napríklad tým, že prejdete na Ovládací panel \> Odinštalovať program. Ak sa vyskytnú problémy, odinštalujte ju pomocou [nástroja Microsoft Support and Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

4. Na serveri RDS sa prihláste do Centra spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte aplikácie Microsoft 365 apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Po nainštalovaní balíka Office ***sa neotvárajte ani neprihlasujte*** do žiadnych aplikácií balíka Office.

6. Na serveri RDS, povoliť aktiváciu zdieľaného počítača úpravou databázy registry pomocou nasledujúcich krokov:

1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku Spustiť. Do poľa Otvoriť zadajte **regedit**a potom kliknite na tlačidlo OK.

2. Po zobrazení výzvy vyberte možnosť Yes (Áno), aby Editor databázy Registry mohol vykonať zmeny v zariadení.

3. V Editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serveri RDS ***sa prihláste ako koncový používateľ*** a [overte, či je zapnutá aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Ďalšie podrobnosti o predpokladoch, pokynoch na nastavenie a pokynoch na prispôsobené inštalácie pomocou nástroja na nasadenie balíka Office nájdete v téme [Nasadenie aplikácií Microsoft 365 pre podniky pomocou služieb vzdialenej pracovnej plochy](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Ak chcete opraviť chyby súvisiace s aktiváciou zdieľaného počítača, pozrite si tému [Riešenie problémov so zdieľanou aktiváciou počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  