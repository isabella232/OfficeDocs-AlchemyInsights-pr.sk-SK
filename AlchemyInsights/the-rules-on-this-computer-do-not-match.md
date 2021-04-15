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
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782967"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidlá v tomto počítači sa nezhodujú

Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite si tému Pravidlá v tomto počítači [sa nezhodujú s pravidlami pre Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tím Outlooku implementuje opravu v rámci zostavy 12928.10000. Oprava sa už nachádza v kanáli Insider Fast a bude sa nachádzať v mesačnom kanáli koncom júna 2020. Po opravenej zostavy sa môže naposledy zobraziť výzva Ktoré pravidlá si chcete ponechať. Po zobrazení výzvy vyberte položku Server, vráťte sa do Outlooku a znova zapnite všetky pravidlá, ktoré boli vypnuté.

Kým nebude k dispozícii oprava, použite toto alternatívne riešenie:

**Alternatívne** riešenie: V posledných hláseniach sa tento problém vyskytol u používateľov, ktorí si klientske pravidlá vytvárali len v počítačovej aplikácii Outlook. Ak problém pretrváva, zvážte odstránenie pravidiel a potom pravidlá vytvárajte a upravujte iba v aplikácii OWA (Outlook Web App), kým sa problém nevyrieši.

Ak nie je možné odstrániť pravidlá manuálne, môžete spustiť príkaz programu Outlook pri spustení Outlooku spustením príkazu Outlook.exe /cleanrules. Týmto sa odstránia pravidlá klienta aj servera. Odstránia sa všetky pravidlá pre všetky kontá v profile Outlooku. Tento príkaz sa ďalej z dokumentuje v článku Prepínače príkazového riadka.

