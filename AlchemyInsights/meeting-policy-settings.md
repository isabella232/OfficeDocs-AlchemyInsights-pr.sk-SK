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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925180"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Spravovanie politík schôdzí v Microsoft Teams

**Poznámka: Zmeny politiky sa prejavia pre používateľov do 24 hodín.** Je možné, že ihneď nebudete môcť vykonať zmeny v novovytvorených politikách. Počkajte 4 hodiny a skúste znova upraviť novovytvoreú politiku.

Politiky schôdzí sa používajú na ovládanie funkcií dostupných pre účastníkov schôdze na schôdze naplánované používateľmi vo vašej organizácii. Niektoré funkcie politík schôdzí sa možno ešte neimplementovať do Centra spravovania pre Teams (tieto sú v dokumentácii označené ako "čoskoro k dispozícii"). V tomto prípade alebo ak sa vám zobrazuje chybové hlásenie, napríklad "Politiku nie je možné aktualizovať hneď, ale skúste to znova neskôr" v Centre spravovania pre Microsoft Teams odporúčame použiť Prostredie PowerShell na vytvorenie alebo úpravu politík Teams schôdzí. 

Ďalšie informácie o politikách schôdzí nájdete v týchto zdrojoch:

- Ďalšie informácie o vytváraní politík, zmenách a priraďovaní používateľov k politike nájdete v téme Správa politík [schôdzí v Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Ak chcete vykonávať zmeny politiky pomocou rutín typu cmdlet prostredia PowerShell, pozrite [si Teams PowerShell Overview.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Na ďalšie politiky [schôdzí je Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams prostredia PowerShell. 
    - Ďalšie informácie [nájdete v dokumentácii rutiny typu cmdlet *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

