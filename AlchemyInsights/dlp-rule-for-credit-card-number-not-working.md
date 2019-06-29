---
title: DLP pravidlo číslo kreditnej karty nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389592"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problémy s čísla kreditných kariet

Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúcich **Čísla kreditnej karty** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre spustenie DLP politiky, keď sa vyhodnotí. Napríklad pre **kreditnú kartu politiky** nakonfigurované s 85% úrovni spoľahlivosti, takto hodnotia a musí zistiť pravidlo spustiť:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môže byť formátovaný alebo neformátovaný (dddddddddddddddd) a musí vyhovieť skúške Luhn.

- **[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi komplexný a robustný vzor, ktorý detekuje karty od všetkých významných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekové poukážky a karty stravník.

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politiky je 85% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:

  - Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.

  - Je splnená jedna z nasledujúcich možností:

  - Nájsť slovo od Keyword_cc_verification.

  - Kľúčové slovo z Keyword_cc_name nájdených

  - Funkcia Func_expiration_date zistí dátum správny dátum formát.

  - Kontrolný prechádza

    Napríklad nasledujúca ukážka by spúšť pre DLP politika číslo kreditnej karty:

  - Víza: 4485 3647 3952 7352
  
  - Platnosť: 2/2009

Pre viac informácií o čo je nevyhnutné pre **Číslo kreditnej karty** je možné pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií vyhľadajte kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  