---
title: Inventár zariadenia Intune
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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014087"
---
# <a name="intune-device-inventory"></a>Inventár zariadenia Intune

Server Devices blade poskytuje správcom prehľad o zariadeniach v rámci správy v rámci služby Intune v závislosti od zariadenia. Zobrazené informácie zahŕňajú: hardvér, zistené aplikácie, stav súladu zariadení a stav konfigurácie zariadenia.

Údaje inventára hardvéru a objavených aplikácií sa zhromažďujú v sedemdňovom cykle. Aplikácie a konkrétne prvky hardvéru sa hlásia odlišne v závislosti od operačného systému zariadenia a od toho, či zariadenie vlastníte osobne alebo podnikové zariadenie.

Ďalšie informácie nájdete v téme [Zobrazenie podrobností o zariadení v intune.](https://docs.microsoft.com/intune/device-inventory)

**Najčastejšie otázky**

Otázka: Nedoručiť sa úplný zoznam aplikácií, ktoré sa nachádzajú v zariadeniach zaregistrovaných v Windows Intune. prečo nie?

A: V tejto dobe sú pre počítače so systémom Windows 10 označené ako firemné aplikácie iba moderné aplikácie. Intune nezhromažďuje informácie o aplikáciách Win32 nainštalovaných v týchto zariadeniach.

Otázka: Prečo sa telefónne čísla nezhromažďujú zo všetkých zariadení?

A: Telefóny kategorizované ako firemné zariadenia v intune nie sú označené ich celým telefónnym číslom, ak napríklad spustíte správu o inventári mobilného zariadenia. Telefónne čísla pre vaše vlastné zariadenia sú vždy čiastočne maskované hviezdičkami (****) a zobrazujú sa len posledné štyri číslice.