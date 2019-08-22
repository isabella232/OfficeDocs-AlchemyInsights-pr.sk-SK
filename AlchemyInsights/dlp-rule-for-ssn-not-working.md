---
title: DLP pravidlo pre SSN nefunguje
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529884"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problémy s rodné čísla

Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **Číslo sociálneho poistenia (SSN)** , pri použití typu citlivých informácií v službách Office 365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre to, čo hľadá DLP politiky. 
  
Napríklad SSN politiky nakonfigurované s 85% úrovni spoľahlivosti, takto sa vyhodnocujú a musí zistiť pravidlo spustiť:
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 číslic, ktoré môže byť formátovaný alebo neformátovaný vzor

- **[Vzorka:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie Hľadať SSNs v štyroch rôznych modelov:

  - Func_ssn nájde SSNs pred-2011 výrazné formátovanie, ktoré sú formátované pomlčky alebo medzery (ddd-dd-dddd alebo ddd dd dddd)

  - Func_unformatted_ssn nájde SSNs pred-2011 silné formátovania, ktoré sú naformátovaná ako deväť po sebe idúcich číslic (ddddddddd)

  - Func_randomized_formatted_ssn nájde SSNs roku 2011, ktoré sú formátované pomlčky alebo medzery (ddd-dd-dddd alebo ddd dd dddd)

  - Func_randomized_unformatted_ssn nájde SSNs roku 2011, ktorá je naformátovaná ako deväť po sebe idúcich číslic (ddddddddd)

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, neexistuje žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politiky je 85% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:

  - [Funkcia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) nájde obsah, ktorý zodpovedá vzoru.

  - Nájsť slovo od [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Obsahuje príklady kľúčových slov: *sociálne zabezpečenie, sociálne zabezpečenie #, Soc Sec, SSN* . Napríklad nasledujúca ukážka by vyvolať DLP SSN politiky: **SSN: 489-36-8350**
  
Pre viac informácií o čo je potrebné pre SSNs majú byť zistené pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií pozrite sa na SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  