---
title: Dynamics 365 - zle Dashboard zobrazuje v Dynamics 365 jednotné rozhranie
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528566"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Zle dashboard zobrazuje v Dynamics 365 jednotné rozhranie

Existuje niekoľko dôvodov, prečo môžete vidieť odlišné dashboard než očakávate:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Používateľ má nastaviť predvolenú používateľskú tabuľu 

Zvyčajne môžete identifikovať užívateľa predvolenú tabuľu je nastavená, ak tlačidlo **Nastaviť ako predvolené** neukazuje v dashboard panel príkazov. Predvolenú používateľskú tabuľu prepíšu všetky ostatné predvolené tabule, aj keď používateľ predvolenú tabuľu nie je v aktuálnej aplikácii.

Použiť nasledovné riešenie na odstavenie ich predvolenú tabuľu.

1. Vytvoriť nový osobný dashboard.

2. Nastaviť že nový dashboard ako používateľom predvolený program.

3. Odstránenie tejto tabule.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Panel je nastavený v sitemap

Možno ste nastavili organizácie predvolenú tabuľu výberom tabule a položky "Nastaviť ako predvolené" pod "Prispôsobenie systému". Ale tabuľa definovaná v návrhárovi sitemap budú mať prednosť pred túto tabuľu, ak používateľ má prístup k nemu.

Aby užívatelia panel ste nastavili ako predvolené nastavenie organizácie, môžete buď:

* Nastaví túto tabuľu v sitemap

* Odstrániť prístup na sitemap definované tabuľu pre tých užívateľov
