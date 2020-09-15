---
title: Pravidlo DLP pre číslo bankového účtu USA nefunguje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679311"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problémy s DLP s číslami bankových kont USA

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s číslami bankových kont USA**

Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo bankového účtu USA** pri použití údajového typu DLP s citlivými informáciami v službe O365? Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá, keď je vyhodnotená.
  
Napríklad pre politiku **číslo bankového účtu USA** nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic

- **[Vzorka:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 po sebe idúcich číslic.

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Politika DLP je 75% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru

  - Nájde sa kľúčové slovo z Keyword_usa_Bank_Account.

    Pre politiku **bankového konta USA** by sa napríklad spustila nasledujúca vzorka: kontrola konta 78344011

Ďalšie informácie o tom, čo sa vyžaduje pri zisťovaní **čísla bankového konta v USA** , nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií vyhľadávajú číslo bankového účtu USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .
  
Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  