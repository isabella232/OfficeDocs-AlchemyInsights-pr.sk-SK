---
title: Pravidlo DLP pre SSN nefunguje
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004997"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problémy DLP s číslami sociálneho zabezpečenia

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy DLP s SSNs**

Máte problémy s politikami ochrany pred stratou údajov **(DLP),** ktoré nefungujú pre obsah obsahujúci číslo sociálneho zabezpečenia **(SSN)** pri používaní typu citlivých informácií v Microsoft 365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o obsahu politiky DLP. 
  
Napríklad pri politike SSN nakonfigurovanej s úrovňou spoľahlivosti 85 % sa vyhodnotia nasledujúce údaje a musia sa zistiť, aby sa toto pravidlo spustilo:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, ktoré môžu byť vo formátovanom alebo neformátovanom vzore

- **[Vzorka:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie hľadia siete SSNs v štyroch rôznych vzoroch:

  - Func_ssn nájde názvy SSN so silným formátovaním pred rokom 2011, ktoré sú formátované pomocou pomlčiek alebo medzier (ddd-dd-dddd OR ddd dd dddd)

  - Func_unformatted_ssn nájde čísla SSN so silným formátovaním pred rokom 2011, ktoré nie sú naformátované ako deväť po sebe idúcich číslic (dddddddddd)

  - Func_randomized_formatted_ssn nájde názvy SSN po roku 2011, ktoré sú formátované pomocou pomlčiek alebo medzier (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn nájde čísla SSN po roku 2011, ktoré nie sú naformátované na deväť po sebe idúcich číslic (ddddddddd)

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Politika DLP si je na 85% istá, že sa zistil tento typ citlivej informácie, ak v blízkosti 300 znakov:

  - Funkcia [vyhľadá Func_ssn,](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) ktorý zodpovedá vzoru.

  - Nájde sa kľúčové [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) kľúčové slovo z tejto Keyword_ssn. Príklady kľúčových slov: *Social Security, Social Security#, Soc Sec ,SSN.* Napríklad nasledujúca ukážka by spustila politiku DLP SSN: **SSN: 489-36-8350**
  
Ďalšie informácie o tom, čo sa vyžaduje na to, aby sa pri obsahu zistili siete [SSNs,](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) nájdete v nasledujúcej časti tohto článku: Čo typy citlivých informácií hľadať v rámci SSN
  
Ak používate iný vstavaný typ citlivých informácií, informácie potrebné pre iné typy informácií nájdete v nasledujúcom článku: Čo [typy citlivých informácií hľadať](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  