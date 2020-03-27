---
title: Pravidlo DLP pre číslo bankového účtu USA nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977177"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problémy s USA čísla bankových účtov

**Dôležité**: počas týchto nebývalé časy, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné-navštívte [SharePoint Online dočasné funkcie úpravy](https://aka.ms/ODSPAdjustments) pre viac informácií.

**DLP problémy s USA čísla bankových účtov**

Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo bankového účtu USA** pri použití typu DLP citlivé informácie v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politika hľadá, keď je hodnotená.
  
Napríklad v prípade politiky **čísla bankového účtu USA** nakonfigurovanej s úrovňou spoľahlivosti 85% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo, ktoré sa má spustiť:
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 číslic

- **[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 po sebe idúcich číslic.

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Politika DLP je 75% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru

  - Našiel sa kľúčové slovo z Keyword_usa_Bank_Account.

    Napríklad nasledujúca vzorka by spúšť pre **americké číslo bankového účtu** politiky: kontrola účtu 78344011

Ďalšie informácie o tom, čo je potrebné pre **číslo bankového účtu USA** , ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií pozrite sa na číslo bankového účtu USA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  