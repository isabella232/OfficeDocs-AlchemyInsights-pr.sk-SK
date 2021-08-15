---
title: 'Chyba: Pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981128"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidlá v tomto počítači sa nezhodujú

Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite si tému Pravidlá v tomto počítači [sa nezhodujú s pravidlami pre Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Skupina Outlook implementuje opravu v rámci zostavy 12928.10000. Oprava sa už nachádza v kanáli Insider Fast a bude sa nachádzať v mesačnom kanáli koncom júna 2020. Po opravenej zostavy sa môže naposledy zobraziť výzva Ktoré pravidlá si chcete ponechať. Po zobrazení výzvy vyberte položku Server a potom sa vráťte Outlook znova a znova zapnite všetky pravidlá, ktoré boli vypnuté.

Kým nebude k dispozícii oprava, použite toto alternatívne riešenie:

**Alternatívne** riešenie: V posledných hláseniach sa tento problém vyskytol u ľudí, ktorí pravidlá klienta vytvárali Outlook počítači. Ak problém pretrváva, zvážte odstránenie pravidiel a potom pravidlá vytvárajte a upravujte iba v aplikácii OWA (Outlook Web App), kým sa problém nevyrieši.

Ak nie je možné odstrániť pravidlá manuálne, môžete Outlook spustiť príkaz pri spustení Outlook spustením príkazu Outlook.exe /cleanrules. Týmto sa odstránia pravidlá klienta aj servera. Odstránia sa všetky pravidlá pre všetky kontá v Outlook profile. Tento príkaz sa ďalej z dokumentuje v článku Prepínače príkazového riadka.

