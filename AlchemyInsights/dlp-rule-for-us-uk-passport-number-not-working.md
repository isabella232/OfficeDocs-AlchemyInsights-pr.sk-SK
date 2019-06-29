---
title: DLP pravidlo pre USA / UK číslo pasu nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389556"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP - USA / UK čísla pasov

Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **USA / číslo pasu Spojeného kráľovstva** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre čo DLP politiky hľadá, keď sa vyhodnotí.
  
Napríklad pre **USA / číslo pasu Spojeného kráľovstva** politika nakonfigurovaná s hrdosťou úroveň 75%, tieto sa vyhodnocujú a musí byť zistené pravidla vyvolať
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deväť číslic

- **[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deväť po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, neexistuje žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politiky je 75% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:

  - Funkcia Func_usa_uk_passport nájde obsah, ktorý zodpovedá vzoru.

  - Nájsť slovo od Keyword_passport.

    Napríklad nasledujúca ukážka by spúšť pre **USA / číslo pasu Spojeného kráľovstva** politiky: pas USA číslo 123456789

Pre viac informácií o čo je nevyhnutné pre USA / UK pasové údaje sa vyhľadávajú pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [čo citlivé druhy informácií vzhľad pre USA / číslo pasu Spojeného kráľovstva](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  