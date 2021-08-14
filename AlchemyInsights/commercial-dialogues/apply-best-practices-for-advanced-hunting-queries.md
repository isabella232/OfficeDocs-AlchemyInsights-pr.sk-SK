---
title: Použitie najvhodnejších postupov pre pokročilé dotazy na vlaňajšie
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930148"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Použitie najvhodnejších postupov pre pokročilé dotazy na vlaňajšie

Ak chcete získať výsledky rýchlejšie a vyhnúť sa časovým limitom počas spúšťania zložitých dotazov, použite tieto osvedčené postupy:

- Pri pokuse o nové dotazy vždy použite limit, aby ste sa vyhli príliš veľkým množinám výsledkov. Môžete tiež `count` vykonať počiatočné hodnotenie veľkosti súboru výsledkov.
- Najskôr použite filtre času. V ideálnom prípade dotazy obmedzte na sedem dní.
- Na začiatku dotazu hneď za filtrom času pridajte filtre, ktoré by mali odstrániť väčšinu údajov.
- Pri hľadaní celých tokenov použite `has` operátor namiesto `contains` operátora .
- Spustite radšej vyhľadávanie v konkrétnom stĺpci, nie vo všetkých stĺpcoch.
- Pri spájaní tabuliek najprv zadajte tabuľku s menším počtom riadkov.
- `project` len potrebné stĺpce z tabuliek, ktoré ste pripojili.

Ďalšie informácie nájdete v téme Osvedčené [postupy týkajúce sa rozšírených dotazov na vyhľadávanie.](https://go.microsoft.com/fwlink/?linkid=2144812)
