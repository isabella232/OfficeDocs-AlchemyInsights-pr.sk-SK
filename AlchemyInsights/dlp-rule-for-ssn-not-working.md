---
title: Pravidlo DLP pre SSN nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788717"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problémy s číslami sociálneho zabezpečenia

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP problémy s SSNs**

Máte problémy s **Zabránenie strate údajov (DLP)** nepracuje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní citlivé informácie typu v Microsoft 365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politiky hľadá. 
  
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
  