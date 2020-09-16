---
title: Inventár zariadenia služby Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667893"
---
# <a name="intune-device-inventory"></a>Inventár zariadenia služby Intune

Blade zariadenia poskytuje správcovi prehľad o zariadeniach v rámci správy v službe Intune na základe jednotlivých zariadení. Zobrazené informácie zahŕňajú: hardvér, nájdené aplikácie, stav súladu zariadenia a stav konfigurácie zariadenia.

Údaje o zásobách pre hardvér a nájdené aplikácie sa zhromažďujú v priebehu siedmich dní cyklu. Nahlásené aplikácie a špecifické prvky hardvéru sa líšia v závislosti od operačného systému zariadenia a od toho, či je zariadenie osobne alebo podnikovo vlastnené.

Ďalšie informácie nájdete v téme [Zobrazenie podrobností o zariadení v službe Intune](https://docs.microsoft.com/intune/device-inventory).

**Najčastejšie otázky**

Otázka: Neprijímam úplný zoznam aplikácií, ktoré sú prítomné v zariadeniach s Windowsom Intune. prečo nie?

A: v súčasnosti sú na počítačoch s Windowsom 10, ktoré sú identifikované ako podnikové zariadenia, uvedené len moderné aplikácie. Intune nezhromažďuje informácie o aplikáciách Win32 nainštalovaných v týchto zariadeniach.

Otázka: prečo sa nezhromažďujú telefónne čísla zo všetkých zariadení?

A: telefóny kategorizované ako podnikové zariadenia v službe Intune nie sú identifikované s úplným telefónnym číslom, napríklad keď spustíte zostavu inventára mobilného zariadenia. Telefónne čísla s prihlásením do vlastných zariadení sú vždy čiastočne zamaskované hviezdičkou (* * * *) a zobrazia sa iba posledné štyri číslice.