---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977213"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problémy s číslami kreditných kariet

**Dôležité**: počas týchto nebývalé časy, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné-navštívte [SharePoint Online dočasné funkcie úpravy](https://aka.ms/ODSPAdjustments) pre viac informácií.

**DLP problémy s číslami kreditných kariet**

Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo kreditnej karty** pri použití DLP citlivé informácie typu v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP, keď je hodnotená. Napríklad pri **politike kreditnej karty** nakonfigurovanej s úrovňou spoľahlivosti 85% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo, ktoré sa má spustiť:
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátovaný (dddddddddddddddd) a musí prejsť Luhn test.

- **[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty zo všetkých hlavných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekové karty, a Diner karty.

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_credit_card vyhľadá obsah zodpovedajúci vzoru.

  - Je splnená jedna z nasledujúcich možností:

  - Našiel sa kľúčové slovo z Keyword_cc_verification.

  - Kľúčové slovo z Keyword_cc_name sa nachádza

  - Funkcia Func_expiration_date nájde dátum v správnom formáte dátumu.

  - Kontrolný súčet prejde

    Napríklad nasledujúca vzorka by spúšťač DLP číslo kreditnej karty:

  - Vízum: 4485 3647 3952 7352
  
  - Uplynie: 2/2009

Ďalšie informácie o tom, čo je potrebné pre **číslo kreditnej karty** , ktoré sa majú zistiť pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií Hľadať kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  