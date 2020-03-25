---
title: Pravidlo DLP pre SSN nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932550"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problémy s číslami sociálneho zabezpečenia

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

**DLP problémy s SSNs**

Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní citlivé informácie typu v balíku Office 365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politiky hľadá. 
  
Napríklad pre politiku SSN nakonfigurovaný s úrovňou spoľahlivosti 85%, sú vyhodnotené a musia byť detekované pre pravidlo spustiť:
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 číslic, ktoré môžu byť vo formáte alebo neformátovaný vzor

- **[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie Hľadať SSNs v štyroch rôznych vzorov:

  - Func_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)

  - Func_unformatted_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)

  - Func_randomized_formatted_ssn nájde post-2011 SSNs, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)

  - Func_randomized_unformatted_ssn nájde post-2011 SSNs, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - [Funkcia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) vyhľadá obsah zodpovedajúci vzoru.

  - Našiel sa kľúčové slovo z [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Príklady kľúčových slov zahŕňa: *sociálne zabezpečenie, sociálne zabezpečenie #, SoC SEC, SSN* . Napríklad nasledujúca vzorka by vyvolať DLP SSN politiky: **SSN: 489-36-8350**
  
Ďalšie informácie o tom, čo je potrebné pre SSNs byť detekovaný pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií Hľadať SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  