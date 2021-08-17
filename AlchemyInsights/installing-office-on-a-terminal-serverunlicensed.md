---
title: Inštalácia balíka Office na terminálovom serveri – bezlicencovej
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
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055173"
---
# <a name="installing-office-on-a-terminal-server"></a>Inštalácia Office na terminálovom serveri

Na nasadenie Aplikácie Microsoft 365 pre veľké organizácie na Windows serveri pomocou služieb vzdialenej pracovnej plochy (RDS), predtým nazývané terminálové služby:
  
- Musíte mať predplatné na Microsoft 365, ktoré zahŕňa Aplikácie Microsoft 365 pre veľké organizácie, napríklad Office 365 Enterprise E3 alebo Enterprise E5. Tieto Aplikácie Microsoft 365 pre podnikateľov plány Aplikácie Microsoft 365 pre podnikateľov Premium plány nezahŕňajú Aplikácie Microsoft 365 pre veľké organizácie.

- Aktiváciu zdieľaného [počítača je potrebné zapnúť.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Ak chcete nainštalovať inštaláciu Aplikácie Microsoft 365 pre veľké organizácie rds z aplikácie Centrum spravovania služby Microsoft 365, ***ktorá používa predvolené*** nastavenia inštalácie, postupujte podľa nasledujúcich krokov.

> [!TIP]
> Môžete si tiež stiahnuť a spustiť aplikáciu [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať balík Aplikácie Microsoft 365 pre veľké organizácie v režime aktivácie zdieľaného počítača.
  
1. Skontrolujte, Microsoft 365 máte predplatné. [Zistite, ako na to](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. V prípade potreby prejdite na iné Microsoft 365 predplatné. [Zistite, ako na to](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ak Office nainštalované na serveri RDS pomocou iných predplatných Microsoft 365, odinštalujte ho. Môžete to urobiť napríklad tak, že v ovládacom paneli \> odinštalujete program. Ak sa [u vás Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) odinštalujte ho pomocou služby Microsoft.

4. Na serveri RDS sa prihláste do aplikácie Centrum spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte Aplikácie Microsoft 365 pre veľké organizácie](https://portal.office.com/OLS/MySoftware.aspx).

5. Po Office aplikácie ***neotvorte žiadne*** aplikácie balíka Office ani sa do Office prihlásiť.

6. Na serveri RDS povoľte aktiváciu zdieľaného počítača úpravou databázy Registry pomocou týchto krokov:

1. Kliknite pravým tlačidlom Windows tlačidlo myši v ľavom dolnom rohu obrazovky a vyberte položku Spustiť. Do poľa Otvoriť zadajte príkaz **regedit** a potom vyberte tlačidlo OK.

2. Keď sa zobrazí výzva, aby ste editoru databázy Registry umožnili vykonávať zmeny v zariadení, vyberte možnosť Áno.

3. V Editore databázy Registry pridajte hodnotu **reťazca SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serveri RDS sa ***prihláste ako koncový používateľ a*** [overte, či je povolená aktivácia zdieľaného počítača Aplikácie Microsoft 365 pre veľké organizácie.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Ďalšie podrobnosti o predpokladoch, pokynoch na nastavenie a návode na prispôsobenie inštalácií pomocou nástroja na nasadenie balíka Office nájdete v téme Nasadenie Aplikácie Microsoft 365 pre veľké organizácie pomocou služieb vzdialenej [pracovnej plochy.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Ak chcete opraviť chyby súvisiace s aktiváciou zdieľaného počítača, pozrite si tému [Riešenie problémov s aktiváciou zdieľaného počítača,](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)ktorá Aplikácie Microsoft 365 pre veľké organizácie.
  