---
title: 1490 – riešenie problémov – eDiscovery – zlyhanie
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277840"
---
# <a name="troubleshoot-content-search-errors"></a>Riešenie chýb vyhľadávania obsahu

Vyskytli sa problémy pri vyhľadávaní obsahu alebo pri exportovaní výsledkov vyhľadávania?

Zobrazuje sa vám napríklad nasledovné pri spustení vyhľadávania?

- CS008 alebo CS012 chyby

- Chyby na serveri zaneprázdnený/timeout

- Vyskytla sa chyba aplikácie

Alebo pri vyhľadávaní alebo exportovaní výsledkov z veľkého počtu poštových schránok (cez 100 000 poštových schránok) sa zobrazujú chyby exportu?

Pri týchto typoch chýb skúste zopakovať hľadanie umiestnení obsahu, ktoré zlyhali. Ďalšie informácie nájdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Ak exportujete viac než 100K poštových schránok, budete musieť použiť nasledujúce prostredie PowerShell na stiahnutie výsledkov exportu:  [exportovanie výsledkov z viac ako 100k poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
