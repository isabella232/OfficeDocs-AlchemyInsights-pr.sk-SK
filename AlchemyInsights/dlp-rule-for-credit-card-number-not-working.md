---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704216"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problémy s číslami kreditných kariet

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

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
  