---
title: DLP pravidlo pre číslo kreditnej karty nefunguje
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005105"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problémy s DLP číslami kreditných kariet

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP číslami kreditných kariet**

Máte problémy s ochrana pred stratou údajov **(DLP)** pri používaní typu citlivých informácií DLP v O365 s obsahom obsahujúcim číslo kreditnej karty?  Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP pri vyhodnocovaní. Napríklad pri politike kreditnej karty nakonfigurovanej na úrovni spoľahlivosti 85 % sa vyhodnotia nasledujúce pravidlá **a** musia sa zistiť, aby sa toto pravidlo spustilo:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátované (ddddddddddd) a musia prejsť cez Luhnov test.

- **[Vzorka:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veľmi zložitý a robustný vzor, ktorý zisťuje karty všetkých hlavných svetových značiek vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekových poukazov a dinerových kariet.

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Áno, Luhnov kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Politika DLP si je na 85% istá, že sa zistil tento typ citlivej informácie, ak v blízkosti 300 znakov:

  - Funkcia vyhľadá Func_credit_card, ktorý zodpovedá vzoru.

  - Jedna z nasledujúcich platí:

  - Nájde sa kľúčové slovo Keyword_cc_verification kľúčové slovo z tejto lokality.

  - Nájde sa kľúčové Keyword_cc_name z

  - Funkcia Func_expiration_date dátum v správnom formáte dátumu.

  - Kontrolný súčet prejde

    Napríklad nasledujúca ukážka by spustila politiku číslovania kreditných kariet DLP:

  - Visa: 4485 3647 3952 7352
  
  - Platnosť uplynie: 2.2.2009

Ďalšie informácie o tom,  čo sa vyžaduje na to, aby sa zistilo číslo kreditnej karty v obsahu, nájdete v nasledujúcej časti tohto článku: Čo typy citlivých informácií hľadať po kliknutí na položku Kreditná [karta#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Ak používate iný vstavaný typ citlivých informácií, informácie potrebné pre iné typy informácií nájdete v nasledujúcom článku: Čo [typy citlivých informácií hľadať](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  