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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679384"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problémy s DLP s číslami sociálneho zabezpečenia

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s čísla SSN**

Vyskytli sa problémy so zabezpečením **ochrany pred únikom údajov (DLP)** , ktoré nefungujú s obsahom, ktorý obsahuje **číslo sociálneho zabezpečenia (SSN)** pri použití citlivého typu informácií v Microsoft 365? Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo sa pri vyhľadávaní politiky DLP nachádza. 
  
Napríklad pre politiku SSN nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť nasledovné:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, ktoré môžu byť formátované alebo nenaformátované

- **[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie vyhľadávajú čísla SSN v štyroch rôznych vzorcoch:

  - Func_ssn nájde čísla SSN s vopred 2011 silným formátovaním s pomlčkami alebo medzerami (DDD – DD-dddd alebo DDD DD dddd)

  - Func_unformatted_ssn nájde čísla SSN s formátovaním pre-2011 silné formátovanie, ktoré nie je formátované ako deväť po sebe idúcich číslic (ddddddddd)

  - Func_randomized_formatted_ssn nájde čísla SSN post-2011, ktoré sú formátované pomlčkami alebo medzerami (DDD – DD-dddd alebo DDD DD dddd)

  - Func_randomized_unformatted_ssn nájde čísla SSN post-2011, ktoré nie sú formátované ako deväť po sebe idúcich číslic (ddddddddd)

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Politika DLP je 85% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - [Funkcia Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nájde obsah, ktorý zodpovedá vzoru.

  - Nájde sa kľúčové slovo z [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Príklady kľúčových slov zahŕňajú:  *sociálne zabezpečenie, sociálna bezpečnosť #, SoC SEC, SSN*  . Pre politiku DLP SSN by sa napríklad spustila nasledujúca vzorka: **SSN: 489-36-8350**
  
Ďalšie informácie o tom, čo sa vyžaduje pre čísla SSN, ktoré sa majú zistiť pre svoj obsah, nájdete v tejto časti tohto článku: [Aké typy citlivých informácií vyhľadávajú čísla SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  