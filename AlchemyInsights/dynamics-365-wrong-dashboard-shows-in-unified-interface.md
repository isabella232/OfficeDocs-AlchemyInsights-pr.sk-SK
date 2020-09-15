---
title: Dynamics 365 – nesprávna tabuľa sa zobrazuje v systéme Dynamics 365 Unified Interface
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711290"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nesprávna tabuľa sa zobrazuje v rozhraní Dynamics 365 Unified Interface

Existuje niekoľko dôvodov, prečo sa môže zobraziť iná tabuľa, než očakávate:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Používateľ nastavil predvolenú tabuľu používateľa 

Zvyčajne je možné identifikovať predvolenú tabuľu používateľa, ak sa na paneli príkazov tabule nezobrazuje tlačidlo **nastaviť ako predvolené** . Predvolenou tabuľou používateľa sa prepíšu všetky ostatné predvolené tabule, a to aj v prípade, že predvolená tabuľa používateľa sa nenachádza v aktuálnej aplikácii.

Ak chcete zrušiť predvolenú tabuľu, použite toto alternatívne riešenie.

1. Vytvorte novú osobnú tabuľu.

2. Nastavte novú tabuľu ako predvolenú používateľa.

3. Odstráňte túto tabuľu.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabuľa sa nastavuje v súbore Sitemap

Možno ste nastavili predvolenú tabuľu organizácie výberom tabule a výberom položky nastaviť ako predvolené v časti Prispôsobenie systému. Tabuľa definovaná v návrhárovi Sitemap však bude mať prednosť pred touto tabuľou, ak má k nemu prístup používateľ.

Ak chcete, aby sa používateľom zobrazila tabuľa, ktorú ste nastavili ako predvolenú organizáciu, môžete buď:

* Nastavenie tejto tabule v Sitemap

* Odstránenie prístupu k súboru Sitemap definovaného tabuľa pre týchto používateľov
