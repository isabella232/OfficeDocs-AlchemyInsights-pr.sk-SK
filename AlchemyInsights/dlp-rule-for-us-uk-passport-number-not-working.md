---
title: Pravidlo DLP pre číslo cestovného pasu USA a Spojeného kráľovstva nefunguje
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
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507313"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP - čísla pasov VUSA a Veľkej Británii

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP problémy s číslami pasov uSA a Veľkej Británie**

Máte problémy s **funkciou Ochrana pred únikom údajov (DLP),** ktorá nepracuje pre obsah obsahujúci **číslo pasu USA a Veľkej Británie** pri používaní typu citlivých informácií DLP v systéme O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá pri hodnotení.
  
Napríklad v prípade politiky **čísla pasov USA a Spojeného kráľovstva** nakonfigurovanej s úrovňou spoľahlivosti 75 % sa vyhodnotia nasledujúce možnosti a musí sa zistiť, aby sa pravidlo spustilo.
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deväť číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deväť po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Politika DLP je 75% presvedčená, že zistila tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_usa_uk_passport nájde obsah, ktorý sa zhoduje so vzorom.

  - Nájde sa kľúčové slovo z Keyword_passport.

    Napríklad nasledujúca vzorka by sa spustiť pre **us / UK číslo pasu číslo** politiky: Číslo cestovného pasu USA 123456789

Ďalšie informácie o tom, čo je potrebné pre US / UK Passport číslo, ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať us / UK Passport číslo](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  