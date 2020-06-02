---
title: Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané použitie na RDS, terminálový Server alebo VDI
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507601"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané použitie na RDS, terminálový Server alebo VDI

Nasadenie aplikácií microsoft 365 pre podniky pomocou služby vzdialenej skúsenosti s prácou s počítačom (RDS), predtým s názvom Terminálové služby:
- Musíte mať plán Microsoft 365 For Business alebo plán služieb Office 365, ktorý obsahuje aplikácie Microsoft 365 for enterprise, napríklad Office 365 Enterprise E3 alebo Enterprise E5.
   > [!NOTE] 
   > Plány Aplikácií Microsoft 365 for business a Microsoft 365 Business Premium Standard nezahŕňajú aplikácie Microsoft 365 pre podniky.
- Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Môžete tiež prevziať a spustiť [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 Apps pre podniky v režime aktivácie zdieľaného počítača.

Ďalšie informácie o predpokladoch, pokynoch na nastavenie a pokynoch na prispôsobené inštalácie pomocou nástroja na nasadenie balíka Office nájdete v téme [Nasadenie aplikácií Microsoft 365 pre podniky pomocou služieb vzdialenej pracovnej plochy](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Oprava chýb súvisiacich s aktiváciou zdieľaného počítača:
- Ďalšie [informácie nájdete v téme Riešenie problémov so zdieľaným počítačom pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pozrite si tému [Resetovanie stavu aktivácie služby Aplikácie Microsoft 365 pre veľké organizácie](https://go.microsoft.com/fwlink/?linkid=2109218).

Ak chcete nainštalovať Microsoft 365 Aplikácie pre podniky na RDS z Microsoft 365 admin Center, ***ktorý používa predvolené nastavenie inštalácie,*** postupujte nasledovne:

1.    Skontrolujte, aké predplatné máte. [Prečítajte si, ako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    V prípade potreby prepnite na iné predplatné. [Prečítajte si, ako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Ak je balík Office už nainštalovaný na serveri RDS pomocou iných predplatných od spoločnosti Microsoft, odinštalujte ho. Napríklad tým, že prejdete na **Ovládací panel**  >  **Odinštalovať program**. Ak sa vyskytnú problémy, odinštalujte ju pomocou [nástroja Microsoft Support and Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)
4.    Na serveri RDS sa prihláste do Centra spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte aplikácie Microsoft 365 apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Po nainštalovaní balíka Office ***sa neotvárajte ani neprihlasujte*** do žiadnych aplikácií balíka Office.
6.    Na serveri RDS, povoliť aktiváciu zdieľaného počítača úpravou databázy registry pomocou nasledujúcich krokov:
   1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte **reťazec regedit**a potom vyberte **tlačidlo OK**.
   2. Po zobrazení výzvy vyberte možnosť **Yes (Áno),** aby Editor databázy Registry mohol vykonať zmeny v zariadení.
   3. V Editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveri RDS ***sa prihláste ako koncový používateľ*** a [overte, či je zapnutá aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

