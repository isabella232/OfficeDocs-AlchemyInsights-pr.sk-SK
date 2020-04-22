---
title: Pravidlo DLP pre číslo pasu USA/UK nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715001"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP-USA/UK čísla pasu

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP problémy s USA/UK čísla pasu**

Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **USA/UK číslo pasu** pri použití DLP citlivé informácie typu v službe O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politika hľadá, keď je hodnotená.
  
Napríklad v prípade politiky **čísla pasu USA/Spojeného kráľovstva** nakonfigurovanej s úrovňou spoľahlivosti 75% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo na spustenie
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deväť číslic

- **[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deväť po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Politika DLP je 75% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_usa_uk_passport vyhľadá obsah zodpovedajúci vzoru.

  - Našiel sa kľúčové slovo z Keyword_passport.

    Napríklad nasledujúca vzorka by spúšť pre **USA/UK Passport číslo** politiky: US passport číslo 123456789

Ďalšie informácie o tom, čo je potrebné pre USA/UK číslo pasu, ktoré majú byť detekované pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií hľadať pre nás/UK číslo pasu](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  