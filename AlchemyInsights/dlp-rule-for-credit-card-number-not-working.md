---
title: DLP pravidlo pre číslo kreditnej karty nefunguje
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
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507421"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problémy s číslami kreditných kariet

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP problémy s číslami kreditných kariet**

Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** nefunguje pre obsah obsahujúci **číslo kreditnej karty** pri používaní typu citlivých informácií DLP v systéme O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP pri jej vyhodnocovaní. Napríklad pre **politiku kreditnej karty** nakonfigurovaný s úrovňou spoľahlivosti 85%, sa vyhodnotia nasledovné a musí sa zistiť, aby pravidlo spúšťať:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátované (dddddddddddddddddddd) a musia prejsť Luhnovou skúškou.

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty od všetkých hlavných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekových kariet a kariet stravníkov.

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Áno, kontrolný súčet Luhna.

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Politika DLP je 85% presvedčená, že sa zistil tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.

  - Jedna z nasledujúcich je splnená:

  - Nájde sa kľúčové slovo od Keyword_cc_verification.

  - Kľúčové slovo z Keyword_cc_name sa nachádza

  - Funkcia Func_expiration_date vyhľadá dátum v správnom formáte dátumu.

  - Kontrolný súčet prechádza

    Napríklad nasledujúca vzorka by sa spustiť pre DLP číslo kreditnej karty politiky:

  - Vízum: 4485 3647 3952 7352
  
  - Uplynie: 2/2009

Ďalšie informácie o tom, čo je potrebné pre **číslo kreditnej karty,** ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať kreditnej karty #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  