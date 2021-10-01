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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041021"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasadenie Aplikácie Microsoft 365 pre veľké organizácie na zdieľané používanie v RDS, terminálovom serveri alebo VDI

Ak chcete Aplikácie Microsoft 365 pomocou služieb vzdialenej pracovnej plochy (RDS), predtým terminálových služieb, musíte:

- Ak chcete povoliť protokol TLS 1.2 ako predvolený, použite jednoduchú opravu, ak používate staršiu verziu balíka Windows (napríklad Windows 7 SP1, Windows Server 2008 R2). Jednoduché opravy a ďalšie informácie nájdete v téme Aktualizácia na povolenie [protokolu TLS 1.1 a TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)ako predvolených zabezpečených protokolov v systéme WinHTTP v Windows. 
- máte plán, ktorý zahŕňa Aplikácie Microsoft 365 pre veľké organizácie (predtým Office 365 Plus). Môže to byť napríklad Office 365 E3 alebo Microsoft 365 E5, alebo akýkoľvek plán, ktorý obsahuje počítačovú verziu balíka Project alebo Visio, napríklad Project Plan 3 alebo Visio Plan 2, alebo plán Microsoft 365 Business Premium, ktorý tiež obsahuje Aplikácie Microsoft 365 pre podnikateľov.
- Povoľte aktiváciu zdieľaného počítača. Ďalšie informácie nájdete v téme [Prehľad aktivácie zdieľaného počítača pre Aplikácie Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Poznámka:** Ak chcete Aplikácie Microsoft 365 v režime aktivácie zdieľaného počítača, stiahnite si a spustite [aplikáciu Microsoft Support and Recovery Assistant.](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds) Podrobné informácie o predpokladoch, pokynoch na nastavenie a návode na prispôsobenie inštalácií pomocou nástroja na nasadenie balíka Office nájdete v téme Nasadenie Aplikácie Microsoft 365 pomocou služieb vzdialenej [pracovnej plochy.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Ak chcete opraviť chyby týkajúce sa aktivácie zdieľaného počítača, pozrite si témy:

- [Riešenie problémov s aktiváciou zdieľaného počítača pre Aplikácie Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Resetovať Aplikácie Microsoft 365 pre veľké organizácie stav aktivácie](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ak chcete nainštalovať inštaláciu balíka Aplikácie Microsoft 365 rds z aplikácie Centrum spravovania služby Microsoft 365, ktorá používa predvolené nastavenia inštalácie, postupujte takto:

1. Skontrolujte, Microsoft 365 plán máte. Ďalšie informácie nájdete v téme [Aké predplatné používam?.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. V prípade potreby prejdite na iný Microsoft 365 plán. Ďalšie informácie nájdete v téme [Inovácia na iný plán.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Ak Aplikácie Microsoft 365 na serveri RDS pomocou iných nekompatibilných plánov, odinštalujte ho tak, že v ovládacom **paneli** odinštalujete  >  **program.** Ak sa pri problémoch vyskytuje, odinštalujte [ho stiahnutím služby Microsoft Support and Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Na serveri RDS sa prihláste do služby Centrum spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Po Office aplikácie neotvorte žiadne aplikácie balíka Office ani sa do Office prihlásiť.

1. Na serveri RDS povoľte aktiváciu zdieľaného počítača úpravou databázy Registry:

   1. Kliknite pravým tlačidlom Windows tlačidlo myši v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**. Do poľa Otvoriť zadajte príkaz **regedit** a potom vyberte tlačidlo **OK.**

   1. Po zobrazení výzvy na povolenie editora databázy Registry vykonávať zmeny v zariadení vyberte možnosť **Áno.**

   1. V editore databázy Registry v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením **1.**

1. Na serveri RDS sa prihláste ako koncový používateľ a overte, či je aktivácia zdieľaného počítača zapnutá Aplikácie Microsoft 365. 

   Podrobnosti nájdete v téme [Overenie, či je zapnutá aktivácia zdieľaného počítača Aplikácie Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)