---
title: Obísť lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768455"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Ovládanie nastavení vstupnej haly a úrovne účasti

Ak chcete povoliť všetkým, vrátane dial-in, externých a anonymných používateľov obísť lobby v Microsoft Teams, môžete použiť PowerShell na to. Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tento cmdlet v súčasnosti vyžaduje použitie Skype Business PowerShell modulu. Ak chcete získať nastavenie na používanie tejto rutiny cmdlet, pozrite si [správu politík pomocou prostredia PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Môžete nastaviť novú politiku, ktorú potom budete musieť použiť pre používateľov. Ak upravíte globálnu politiku, ktorá sa automaticky použije pre používateľov. Pre každú zmenu politiky musíte počkať aspoň 4 hodiny a až 24 hodín, kým sa politiky prejavia.

Nezabudnite si prezrieť dokumentáciu nižšie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Pochopenie tímov pre kontrolu politiky lobby

- [Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.

- [Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.

- [Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .

- [Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastaví v **automatickom priznávanie osôb** a **povolenie telefonického pripojenia používateľom obísť vstupnú halu** , keď naplánujú novú schôdzu.

**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams.
