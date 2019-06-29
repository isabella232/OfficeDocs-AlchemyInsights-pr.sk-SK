---
title: Inštalácia office na terminálový Server - bez licencie
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381744"
---
# <a name="installing-office-on-a-terminal-server"></a>Inštalácia balíka Office na terminálový Server

Na nasadenie balíka Office 365 ProPlus na serveri Windows Server pomocou Remote Desktop Services (RDS), pôvodne pomenovaný terminálových služieb:
  
- Musíte mať plán služieb Office 365, ktorý obsahuje Office 365 ProPlus, napríklad Office 365 Enterprise E3 alebo Enterprise E5. Plány Office 365 Business a Office 365 Business Premium nezahŕňajú Office 365 ProPlus.

- Musíte zapnúť [aktiváciou zdieľaný počítač](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ak chcete nainštalovať Office 365 ProPlus na RDS z Office 365 portálu, ** *ktoré používa predvolené nastavenia inštalácie* **, postupujte nasledovne:
  
1. Skontrolujte, aký máte plán služieb Office 365. [Zistite ako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ak potrebné, prepnúť na rôzne Office 365 plánu. [Zistite ako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ak Office je už nainštalovaný na serveri RDS používať iné plány služieb Office 365, odinštalujte ju. Napríklad tým, že pôjdete do ovládacieho panela \> odinštalovať program. Odinštalovať pomocou [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak ste beží do problémov.

4. RDS serveri, prihláste sa na portáli Office 365 konto správcu a [inštaláciu balíka Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Po nainštalovaní balíka Office ** *neotvárajte ani prihlásiť* ** všetky aplikácie balíka Office.

6. Na serveri RDS povoliť aktiváciou zdieľaný počítač úpravou databázy registry pomocou nasledujúcich krokov:

1. Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť. Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.

2. Vybrať áno keď výzva na povolenie Editor databázy Registry zmeny do vášho zariadenia.

3. V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavenie 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serveri RDS ** *Prihlásiť ako koncový používateľ* ** a [overiť, že aktiváciou zdieľaný počítač zapnutá pre Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Viac informácií o predpoklady, pokynov a usmernenia na prispôsobenej inštalácie pomocou nástroja nasadenia Office, nájdete [Nasadenie balíka Office 365 ProPlus pomocou služby vzdialenej pracovnej plochy](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Opraviť chyby súvisiace s aktiváciou zdieľaný počítač nájdete v [článku Riešenie problémov s aktiváciou zdieľaný počítač pre Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  