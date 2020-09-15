---
title: Pravidlo DLP pre US/UK Passport číslo nefunguje
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679239"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s číslami služby DLP – US/UK Passport

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s číslami o pasoch v USA a Spojenom kráľovstve**

Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo cestovného pasu USA/UK** pri použití údajového typu DLP s citlivými informáciami v službe O365? Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá, keď je vyhodnotená.
  
Napríklad pre politiku **číslo Passport USA/UK** nakonfigurovanú s úrovňou spoľahlivosti 75% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deväť číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deväť po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Politika DLP je 75% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Funkcia Func_usa_uk_passport nájde obsah, ktorý zodpovedá vzoru.

  - Nájde sa kľúčové slovo z Keyword_passport.

    Nasledujúca vzorka by napríklad spustila politiku **Passport pre USA a Veľkú Britániu** : US passport Number 123456789

Ďalšie informácie o tom, čo sa vyžaduje pre číslo pasu USA/UK, ktoré sa má zistiť pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií vyhľadávajú číslo cestovného pasu pre USA alebo UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .
  
Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  