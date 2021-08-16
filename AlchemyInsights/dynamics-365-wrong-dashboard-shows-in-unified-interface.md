---
title: Dynamics 365 – nesprávna tabuľa sa zobrazuje v zjednotenom rozhraní Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101497"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>V zjednotenom rozhraní služby Dynamics 365 sa zobrazuje nesprávna tabuľa

Existuje niekoľko dôvodov, prečo sa môže zobraziť iná tabuľa ako očakávaná tabuľa:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Používateľ nastavil predvolenú tabuľu používateľa 

Zvyčajne môžete identifikovať predvolenú tabuľu používateľa, ak sa tlačidlo Nastaviť ako predvolené na paneli príkazov tabule (dashboard) nebude zobrazovať.  Predvolená tabuľa používateľa prepíše všetky ostatné predvolené tabule, a to aj v prípade, že predvolená tabuľa používateľa nie je v aktuálnej aplikácii.

Ak chcete zrušiť nastavenie predvolenej tabule, použite nasledujúce alternatívne riešenie.

1. Vytvorte novú osobnú tabuľu.

2. Nastavte túto novú tabuľu ako predvolenú.

3. Odstráňte túto tabuľu.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabuľa je nastavená v mape lokality

Možno ste nastavili predvolenú tabuľu organizácie výberom tabule a výberom položky Nastaviť ako predvolené v časti Prispôsobiť systém. Tabuľa definovaná v návrhárovi mapy lokality však bude mať prednosť pred touto tabuľou (dashboard), ak k nej má používateľ prístup.

Ak chcete používateľom zobraziť tabuľu, ktorú ste nastavili ako predvolenú organizáciu, môžete:

* Nastavenie tabule (dashboard) v mape lokality

* Odstránenie prístupu k tabuli definovanej pomocou mapy lokality pre týchto používateľov
