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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042859"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa politík schôdzí v programe Microsoft teams

**Poznámka: môže trvať až 24 hodín, kým sa zmeny politiky prejavia pre používateľov.** Pravdepodobne nebudete môcť okamžite vykonať zmeny novovytvorených politík. Počkajte 4 hodiny a pokúste sa znova upraviť novovytvorenú politiku.

Politiky schôdzí sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze, ktoré sú naplánované používateľmi vo vašej organizácii. Niektoré funkcie politiky schôdzí nemusia byť implementované v tíme admin Center zatiaľ (tieto sú označené "pripravujeme" v dokumentácii). V tomto prípade, alebo ak ste získali chybu ako "nemôžeme aktualizovať politiku práve teraz, ale skúste to znova neskôr" v Microsoft teams admin Center, odporúčame použiť PowerShell vytvoriť alebo upraviť tímy stretnutia politiky. 

Ďalšie informácie o politikách schôdzí nájdete v nasledujúcich zdrojoch informácií:

- Informácie o vytváraní politík, vykonaní zmien a priraďovaní používateľov k politike nájdete [v téme Spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Ak chcete vykonať zmeny politiky pomocou rutiny cmdlet prostredia PowerShell, pozrite si [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Musíte použiť [Skype Business PowerShell modul](https://www.microsoft.com/download/details.aspx?id=39366) pre tímy schôdze politiky. 
    - Skontrolujte [*-csteamsmeetingpolicy rutiny cmdlet dokumentáciu](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pre viac informácií.

