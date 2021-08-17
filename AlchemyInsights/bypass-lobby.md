---
title: Obídenie čakáreň
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059611"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Ovládanie nastavení čakáreňa a úrovne účasti v Teams

Ak chcete všetkým vrátane telefonických, externých a anonymných používateľov povoliť obídenie čakáreň **,** použite prostredie PowerShell na vykonanie tejto úlohy. Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Táto rutina typu cmdlet momentálne vyžaduje Skype for Business prostredia PowerShell. Ak chcete nastaviť používanie tejto rutiny typu cmdlet, pozrite si časť [Spravovanie politík prostredníctvom prostredia PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Po nastavení politiky ju budete musieť použiť pre používateľov. alebo, ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov. Pri každej zmene politiky je potrebné počkať aspoň 4 hodiny až **do 24** hodín, kým sa politiky prejavia. 

Pred vykonaním týchto zmien nezabudnite skontrolovať dokumentáciu nižšie, aby ste presne pochopili, čo to umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Vysvetlenie ovládacích Teams politík v čakárni schôdze

Tieto nastavenia ovládajú, ktorí účastníci schôdze pred ich vstupom na schôdzu budú čakať v čakárni, a tiež povolenú úroveň účasti na schôdzi. Pomocou prostredia PowerShell môžete aktualizovať nastavenia politiky schôdze, ktoré ešte neboli implementované (označené ako čoskoro k dispozícii) v Centre spravovania pre Teams schôdze. Nižšie je uvedený príklad rutiny typu cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť čakáreň.

- [Automatické prijatie osôb je](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) politika organizátora, ktorá určuje, či sa ľudia pripájajú k schôdzi priamo alebo počkať v čakárni, kým ich nepripojí overený používateľ.

- [Umožniť](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) anonymným ľuďom začať schôdzu je politika organizátora, ktorá určuje, či sa anonymní ľudia vrátane B2B a federované používatelia môžu pripojiť k schôdzi používateľa bez toho, aby z organizácie používala účasť overený používateľ.

- [Povoliť používateľom](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) telefonickej konferencie obísť čakáreň **(čoskoro** k dispozícii) je politika organizátora, ktorá určuje, či sa používatelia telefonicky pripoja k schôdzi priamo alebo čakajú v čakárni bez ohľadu na nastavenie Automaticky **prijať** ľudí.

- [Možnosť Povoliť organizátorom](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) prepísať nastavenia čakáreň **(čoskoro** k dispozícii) je politika organizátora, ktorá  určuje,  či organizátor schôdze môže prepísať nastavenia čakáreň, ktoré správca nastavil v časti Automaticky prijať osoby a Povoliť používateľom telefonickej konferencie obísť čakáreň pri naplánovaní novej schôdze.

**Poznámka:** Ak [chcete získať úplný prehľad o politikách Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) schôdzí, prečítajte si článok Spravovanie politík Microsoft Teams schôdzí.
