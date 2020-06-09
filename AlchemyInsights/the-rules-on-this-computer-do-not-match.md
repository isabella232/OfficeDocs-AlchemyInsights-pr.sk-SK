---
title: 'Chyba: Pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664261"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidlá v tomto počítači sa nezhodujú

Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite [si pravidlá v tomto počítači nezodpovedajú pravidlám na serveri Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tím programu Outlook implementoval opravu v build 12928.10000. Oprava je už na Insider Fast a pôjde do mesačného kanála na konci júna 2020. Akonáhle budete mať pevnú stavať môžete dostať výzvu "Aké pravidlá chcete zachovať" ešte raz. Po zobrazení výzvy vyberte položku Server a potom sa vráťte do programu Outlook a znova povoľte všetky pravidlá, ktoré boli vypnuté.

Kým oprava je k dispozícii, použite nasledujúce riešenie:

**Riešenie:** V posledných zostavách sa vyskytol problém pre tých, ktorí vytvorili iba pravidlá klienta v pracovnej ploche programu Outlook. Ak sa problém vyskytuje aj naďalej, zvážte odstránenie pravidiel a potom vytvorte a upravte pravidlá iba v aplikácii OWA (Outlook Web App), kým sa problém nevyrieši.

Ak nemôžete odstrániť pravidlá manuálne, môžete spustiť príkaz programu Outlook pri spustení programu Outlook spustením outlook.exe /cleanrules. Tým sa odstránia pravidlá klienta aj servera. Odstráni všetky pravidlá pre všetky kontá v profile programu Outlook. Tento príkaz je ďalej zdokumentovaný v článku prepínače príkazového riadka.

