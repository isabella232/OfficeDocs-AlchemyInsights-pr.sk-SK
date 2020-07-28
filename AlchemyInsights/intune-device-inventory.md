---
title: Intune inventár zariadenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440476"
---
# <a name="intune-device-inventory"></a>Intune inventár zariadenia

Čepeľ Zariadenia poskytuje správcovi prehľad o zariadeniach, ktoré sú pod správou v intune na základe zariadenia. Zobrazené informácie zahŕňajú: Hardvér, Objavené aplikácie, Stav súladu zariadenia a Stav konfigurácie zariadenia.

Údaje o zásobách pre hardvér a objavené aplikácie sa zhromažďujú v sedemdňovom cykle. Aplikácie a konkrétne prvky nahláseného hardvéru sa líšia v závislosti od operačného systému zariadenia a od toho, či je zariadenie osobne alebo vo vlastníctve podniku.

Ďalšie informácie nájdete v téme Zobrazenie [podrobností o zariadení v programe Intune](https://docs.microsoft.com/intune/device-inventory).

**Najčastejšie otázky**

Otázka: Nedostávam úplný zoznam aplikácií prítomných v zariadeniach s Windowsom zaregistrované v intune. prečo nie?

A: V tomto čase sú pre počítače s Windowsom 10, ktoré sú identifikované ako podnikové zariadenia, sú v zozname iba moderné aplikácie. Intune nezhromažďuje informácie o aplikáciách Win32 nainštalovaných v týchto zariadeniach.

Otázka: Prečo sa telefónne čísla nezhromažďujú zo všetkých zariadení?

A: Telefóny kategorizované ako podnikové zariadenia v programe Intune nie sú identifikované s celým telefónnym číslom, keď napríklad spustíte správu o inventári mobilného zariadenia. Telefónne čísla na vlastné zariadenia sú vždy čiastočne zamaskované hviezdičkami (****) a zobrazujú len posledné štyri číslice.