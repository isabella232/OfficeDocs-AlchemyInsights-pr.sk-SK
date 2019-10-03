---
title: Nastavenie politiky schôdzí
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376820"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa politík schôdzí v programe Microsoft teams

Politiky schôdzí sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze, ktoré sú naplánované používateľmi vo vašej organizácii. Niektoré funkcie politiky schôdzí nemusia byť implementované v tíme admin Center zatiaľ (tieto sú označené "pripravujeme" v dokumentácii). V tomto prípade, alebo ak ste získali chybu ako "nemôžeme aktualizovať politiku práve teraz, ale skúste to znova neskôr" v Microsoft teams admin Center, odporúčame použiť PowerShell vytvoriť alebo upraviť tímy stretnutia politiky. 

Ďalšie informácie o politikách schôdzí nájdete v nasledujúcich zdrojoch informácií:

- Informácie o vytváraní politík, vykonaní zmien a priraďovaní používateľov k politike nájdete [v téme Spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Ak chcete vykonať zmeny politiky pomocou rutiny cmdlet prostredia PowerShell, pozrite si [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Musíte použiť [Skype Business PowerShell modul](https://www.microsoft.com/download/details.aspx?id=39366) pre tímy schôdze politiky. 
    - Skontrolujte [*-csteamsmeetingpolicy rutiny cmdlet dokumentáciu](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pre viac informácií.

**Poznámka:** Pre používateľov môže trvať až 24 hodín, kým sa zmeny politiky prejavia. Pravdepodobne nebudete môcť okamžite vykonať zmeny novovytvorených politík. Počkajte 4 hodiny a pokúste sa znova upraviť novovytvorenú politiku. Ak problémy pretrvávajú, vyskúšajte PowerShell.  