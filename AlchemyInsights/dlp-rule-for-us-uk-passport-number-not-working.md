---
title: Pravidlo DLP pre USA/Číslo pasu Spojeného kráľovstva nefunguje
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004961"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP – čísla pasu v USA alebo Spojenom kráľovstve

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy S DLP číslami pasu USA alebo Spojeného kráľovstva**

Máte problémy s ochrana pred stratou údajov **(DLP)** v obsahu obsahujúcom číslo pasu USA **alebo** Spojeného kráľovstva pri používaní typu citlivých informácií DLP v O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá pri vyhodnocovaní.
  
Napríklad pre politiku čísla pasu USA **alebo** Spojeného kráľovstva nakonfigurovanej na úrovni spoľahlivosti 75 % sa vyhodnotí nasledovné a musí sa zistiť, aby sa toto pravidlo spustilo
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deväť číslic

- **[Vzorka:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deväť po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Politika DLP si je na 75% istá, že sa zistil tento typ citlivej informácie, ak v blízkosti 300 znakov:

  - Funkcia vyhľadá Func_usa_uk_passport, ktorý zodpovedá vzoru.

  - Nájde sa kľúčové Keyword_passport kľúčové slovo z Tejto lokality.

    Napríklad nasledujúca ukážka by spustila podmienky pre číslo pasu USA **alebo** Spojeného kráľovstva: číslo pasu v USA 123456789

Ďalšie informácie o tom, čo sa vyžaduje od čísla pasu USA alebo Spojeného kráľovstva v rámci vášho obsahu, nájdete v nasledujúcej časti tohto článku: Čo typy citlivých informácií vyzerajú ako číslo pasu USA alebo Spojeného [kráľovstva](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Ak používate iný vstavaný typ citlivých informácií, informácie potrebné pre iné typy informácií nájdete v nasledujúcom článku: Čo [typy citlivých informácií hľadať](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  