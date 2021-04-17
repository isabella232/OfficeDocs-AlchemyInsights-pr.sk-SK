---
title: Nastavenia politiky schôdze
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825458"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Spravovanie politík schôdzí v aplikácii Microsoft Teams

**Poznámka: Zmeny politiky sa prejavia pre používateľov do 24 hodín.** Je možné, že ihneď nebudete môcť vykonať zmeny v novovytvorených politikách. Počkajte 4 hodiny a skúste znova upraviť novovytvoreú politiku.

Politiky schôdzí sa používajú na ovládanie funkcií dostupných pre účastníkov schôdze na schôdze naplánované používateľmi vo vašej organizácii. Niektoré funkcie politík schôdzí možno ešte nie sú implementované v Centre spravovania pre Teams (tieto sú v dokumentácii označené ako "čoskoro k dispozícii"). V tomto prípade alebo ak sa vám zobrazuje chybové hlásenie, ako napríklad "Politiku nie je možné aktualizovať hneď, ale skúste to znova neskôr" v Centre spravovania služby Microsoft Teams, odporúčame vám použiť prostredie PowerShell na vytvorenie alebo úpravu politík schôdzí cez Teams. 

Ďalšie informácie o politikách schôdzí nájdete v týchto zdrojoch:

- Ďalšie informácie o vytváraní politík, zmenách a priraďovaní používateľov k politike nájdete v téme Správa [politík schôdzí v Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Ak chcete vykonávať zmeny politiky pomocou rutín typu cmdlet prostredia PowerShell, pozrite si [časť Prehľad prostredia PowerShell služby Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Pre politiky schôdzí v [Teams je potrebné použiť modul Skype for Business PowerShell.](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 
    - Ďalšie informácie [nájdete v dokumentácii rutiny typu cmdlet *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

