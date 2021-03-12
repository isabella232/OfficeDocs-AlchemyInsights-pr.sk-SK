---
title: Nastavenie politiky schôdze
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704621"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa politík schôdze v aplikácii Microsoft teams

**Poznámka: Ak chcete, aby sa zmeny politiky prejavili pre používateľov, môže trvať až 24 hodín.** Možno nebudete môcť okamžite vykonávať zmeny v novovytvorených politikách. Počkajte 4 hodiny a pokúste sa znova upraviť novo vytvorenú politiku.

Politiky schôdze sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze pre schôdze, ktoré naplánovali používatelia vo vašej organizácii. Niektoré funkcie politík schôdze sa nemusia implementovať v centre spravovania pre Teams (tieto sú označené ako čoskoro v dokumentácii). V tomto prípade alebo ak sa zobrazuje chybové hlásenie "momentálne nemôžeme aktualizovať politiku, ale skúste to znova neskôr" v centre spravovania služieb Microsoft Teams, odporúčame použiť prostredie PowerShell na vytvorenie alebo úpravu politík schôdze v aplikácii teams. 

Ďalšie informácie o politikách schôdze nájdete v týchto zdrojoch informácií:

- Ďalšie informácie o vytváraní politík, vykonávaní zmien a priradení používateľov k politike nájdete [v téme Správa politík schôdze v aplikácii teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Ak chcete vykonať zmeny politiky pomocou rutiny typu cmdlet prostredia PowerShell, pozrite si tému [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Na politiku schôdze v aplikácii teams musíte použiť [modul PowerShell pre Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) . 
    - Ďalšie informácie nájdete v [dokumentácii k rutine cmdlet *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

