---
title: Použitie najvhodnejších postupov pri rozšírených dotazoch na lov
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696084"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Použitie najvhodnejších postupov pri rozšírených dotazoch na lov

Ak chcete rýchlejšie získavať výsledky a vyhnúť sa timeoutom pri spúšťaní zložitých dotazov, použite tieto najvhodnejšie postupy:

- Pri pokuse o nové dotazy vždy použite limit, aby sa predišlo extrémne vysokým množinám výsledkov. Môžete tiež použiť `count` na vytvorenie počiatočného hodnotenia veľkosti množiny výsledkov.
- Najprv použite časové filtre. V ideálnom prípade Obmedzte dotazy na sedem dní.
- Na začiatku dotazu, hneď po uplynutí časového filtra, pridajte filtre, ktoré sa očakávajú na odstránenie väčšiny údajov.
- Pri vyhľadávaní úplných tokenov použite `has` operátor skôr ako `contains` .
- Spustite vyhľadávanie v konkrétnom stĺpci a nie vo všetkých stĺpcoch.
- Pri pripájaní k tabuľkám najskôr zadajte tabuľku s menším počtom riadkov.
- `project` iba potrebné stĺpce z tabuliek, ku ktorým ste sa pripojili.

Ďalšie informácie nájdete v téme [pokročilé postupy lovu v dotaze](https://go.microsoft.com/fwlink/?linkid=2144812).
