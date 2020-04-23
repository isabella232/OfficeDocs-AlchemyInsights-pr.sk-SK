---
title: Obmedzenie lokality SharePoint Online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742484"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Obmedzenie lokality SharePoint Online na klasický režim

Niektoré organizácie stále vyžadujú klasický režim skúsenosti. Zatiaľ čo neexistujú žiadne plány na odstránenie klasického režimu na granulovanej úrovni, už nie je možné obmedziť celú organizáciu (nájomcu) na klasický režim pre zoznamy a knižnice.

Admin bude mať nasledujúce možnosti spravovať jednotlivé zoznamy a knižnice v klasickom režime pomocou podrobných opt-out prepínače, ktoré poskytujeme na týchto úrovniach:

- kolekcie lokalít
- Stránky
- Zoznam
- Knižnica

Okrem toho zoznamy, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modernými bude stále automaticky prepne do klasického režimu.

Začiatok apríla 1, 2019, proces vypnúť nájomcu úroveň opt out moderného zoznamu a knižníc začne a pokračovať až 31 mája 2019.  Zoznamy a knižnice, ktoré sú v klasickom režime v dôsledku odhlásenia nájomníka sa automaticky posunú na moderné.

Ak požadujete klasický režim, prečítajte si viac informácií [tu](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) a PNP PowerShell inštrukcie [tu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , ktorá opisuje možnosti a nástroje, ktoré môžete použiť dnes používať klasický režim skúsenosti.
