---
title: Obchvatová loby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684965"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Ovládanie nastavení lobby a úrovne účasti v aplikácii teams

Ak chcete všetkým, vrátane telefonických, externých a anonymných používateľov povoliť, aby sa **vyhli vstupnej hale**, použite prostredie PowerShell na vykonanie tejto úlohy. Tu je príklad úpravy globálnej politiky schôdze pre vašu organizáciu.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Táto rutina typu cmdlet v súčasnosti vyžaduje používanie modulu PowerShell v Skype for Business. Ak chcete nastaviť používanie tejto rutiny typu cmdlet, pozrite si tému [Správa politík pomocou prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Po nastavení politiky je potrebné ju použiť pre používateľov. Ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov. Pri každej zmene politiky musíte počkať aspoň **4 hodiny až 24 hodín** , kým sa politiky prejavia. 

Pred vykonaním týchto zmien si prečítajte dokumentáciu nižšie, aby ste presne pochopili, čo to umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informácie o ovládacích prvkoch v lobby schôdze v aplikácii teams

Tieto nastavenia určujú, ktorí účastníci schôdze čakajú v lobby pred prijatím na schôdzu a úrovňou účasti, ktorú sú na schôdzi povolené. Pomocou prostredia PowerShell môžete aktualizovať nastavenia politiky schôdze, ktoré ešte neboli implementované (označené ako "čoskoro") v centre spravovania pre teams. Nižšie nájdete príklad rutiny typu cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.

- [Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú na základe politiky organizátora, ktorá kontroluje, či sa ľudia priamo pripoja k schôdzi alebo čakajú v lobby, až kým neprijmú overeného používateľa.

- [Povoliť anonymným používateľom začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je politika v rámci organizátora, ktorá určuje, či sa majú anonymné osoby vrátane B2B a externých používateľov pripájať k schôdzi používateľa bez overeného používateľa z organizácie v dochádzke.

- [Povoliť používateľom telefonických služieb obísť lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**už čoskoro**) je politika pre organizátora, ktorá kontroluje, či sa osoby, ktoré telefonicky telefonicky pripoja k schôdzi, dostávajú priamo k schôdzi alebo sa v lobby čakajú bez ohľadu na to, či sa **automaticky pripúšťa** nastavenie

- [Ak chcete, aby organizátori](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) prepísali nastavenia lobby (**už čoskoro**), je politika v rámci organizátora, ktorá kontroluje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca **automaticky priznáva ľuďom** a **Povoliť používateľom telefonických služieb obísť lobby** pri plánovaní novej schôdze.

**Poznámka:** Prečítajte si tému [Správa politík schôdze v aplikácii teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) a získajte celkový prehľad o politikách schôdze v aplikácii Microsoft teams.
