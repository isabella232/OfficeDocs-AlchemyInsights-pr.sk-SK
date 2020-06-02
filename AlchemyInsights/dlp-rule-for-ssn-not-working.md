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
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507385"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP otázky s číslami sociálneho zabezpečenia

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s SSNs**

Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** nefunguje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní typu citlivých informácií v microsoft 365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá. 
  
Napríklad pre politiku SSN nakonfigurovaný s úrovňou spoľahlivosti 85%, sa vyhodnotia nasledovné a musí byť detekovaný pre pravidlo spustiť:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, ktoré môžu byť vo formáte formátovaný alebo neformátovaný vzor

- **[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie hľadajú SSN v štyroch rôznych vzoroch:

  - Func_ssn nájde SSN so silným formátovaním pred 2011, ktoré sú formátované pomlčkami alebo medzerami (ddd-ddddd alebo ddd dd dd dd ddddd)

  - Func_unformatted_ssn nájde SSN s pre-2011 silné formátovanie, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)

  - Func_randomized_formatted_ssn nájde ssn po roku 2011, ktoré sú formátované pomlčkami alebo medzerami (ddd-ddddd alebo ddd dd dd ddddd)

  - Func_randomized_unformatted_ssn nájde ssn po roku 2011, ktoré nie sú formátované ako deväť po sebe idúcich číslic (ddddddddd)

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Politika DLP je 85% presvedčená, že sa zistil tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - [Funkcia Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nájde obsah, ktorý sa zhoduje so vzorom.

  - Nájde sa kľúčové slovo z [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Príklady kľúčových slov zahŕňajú: *Sociálne zabezpečenie, sociálne zabezpečenie #, Soc Sec, SSN* . Napríklad nasledujúca vzorka by sa spustiť pre Politiku DLP SSN: **SSN: 489-36-8350**
  
Ďalšie informácie o tom, čo je potrebné pre SSN zistiť obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  