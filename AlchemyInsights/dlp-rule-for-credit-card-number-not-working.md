---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679456"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problémy s DLP s číslami kreditných kariet

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s číslami kreditných kariet**

Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo kreditnej karty** , ak sa v službe O365 používa typ informácií s informáciami o DLP? Ak áno, uistite sa, že obsah obsahuje potrebné informácie na spustenie politiky DLP, keď sa vyhodnotí. Napríklad pre **politiku kreditnej karty** nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť nasledovné:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, ktoré môžu byť formátované alebo nenaformátované (dddddddddddddddd) a musia prejsť testom Luhn.

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty zo všetkých hlavných značiek na celom svete vrátane víz, kariet MasterCard, Discover Card, JCB, American Express, darčekových poukazov a stravníkov.

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Áno, kontrolný súčet Luhn

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Politika DLP je 85% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.

  - Je splnená jedna z nasledujúcich možností:

  - Nájde sa kľúčové slovo z Keyword_cc_verification.

  - Našlo sa kľúčové slovo z Keyword_cc_name

  - Funkcia Func_expiration_date nájde dátum v správnom formáte dátumu.

  - Kontrolný súčet prechádza

    Nasledujúci príklad by sa spustil pre politiku kreditnej karty DLP:

  - Vízum: 4485 3647 3952 7352
  
  - Platnosť uplynie: 2/2009

Ďalšie informácie o tom, čo sa vyžaduje pri zisťovaní **čísla kreditných kariet** pre váš obsah, nájdete v tejto časti tohto článku: informácie o tom, [ktoré typy citlivých informácií vyhľadávajú kreditnú kartu #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  