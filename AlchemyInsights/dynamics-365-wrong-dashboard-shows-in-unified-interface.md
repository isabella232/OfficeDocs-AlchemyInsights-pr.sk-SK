---
title: Dynamics 365-nesprávne Dashboard relácie v Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528566"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nesprávne Dashboard relácie v Dynamics 365 zjednotené rozhranie

Existuje niekoľko dôvodov, prečo sa môže zobraziť iná tabuľa ako tá, ktorú očakávate:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Používateľ nastaviť predvolenú tabuľu používateľa 

Zvyčajne môžete identifikovať predvolenú tabuľu používateľa je nastavená, ak tlačidlo **nastaviť ako predvolené** nezobrazuje v paneli príkazov tabule. Predvolená tabuľa používateľa prepíše všetky ostatné predvolené tabule, a to aj v prípade, že predvolená tabuľa používateľa nie je v aktuálnej aplikácii.

Ak chcete zrušiť nastavenie predvolenej tabule, použite nasledujúce riešenie.

1. Vytvorte novú osobnú tabuľu.

2. Nastaví novú tabuľu ako predvolenú používateľa.

3. Odstrániť túto tabuľu.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabuľa je nastavená v Sitemap

Možno ste nastavili predvolenú tabuľu organizácie výberom tabule a výberom položky "nastaviť ako predvolené" v časti Prispôsobenie systému. Ale Dashboard definované v Sitemap Designer bude mať prednosť pred tejto tabuli, ak má používateľ prístup k nemu.

Ak chcete, aby používatelia videli tabuľu, ktorú ste nastavili ako predvolenú organizáciu, môžete buď:

* Nastaviť, že tabuľa v Sitemap

* Odstránenie prístupu k Sitemap definované Dashboard pre týchto používateľov
