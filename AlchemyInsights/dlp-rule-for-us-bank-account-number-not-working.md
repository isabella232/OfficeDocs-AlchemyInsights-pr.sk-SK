---
title: Pravidlo DLP pre číslo bankového účtu USA nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507349"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problémy s číslami bankových účtov v USA

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP problémy s číslami bankových účtov v USA**

Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** nefunguje pre obsah obsahujúci **číslo bankového účtu USA** pri používaní typu citlivých informácií DLP v službe O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá pri hodnotení.
  
Napríklad pre **politiku čísla bankového konta USA** nakonfigurovaný s úrovňou spoľahlivosti 85%, sa vyhodnotia nasledovné a musí sa zistiť, aby pravidlo spúšťať:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 po sebe idúcich číslic.

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie je tam žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Politika DLP je 75% presvedčená, že zistila tento typ citlivých informácií, ak v blízkosti 300 znakov:

  - Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru

  - Nájde sa kľúčové slovo z Keyword_usa_Bank_Account.

    Napríklad nasledujúca vzorka by sa spustiť pre **politiku čísla bankového účtu USA:** Kontrola účtu 78344011

Ďalšie informácie o tom, čo je potrebné pre **číslo bankového účtu uSA,** ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať číslo bankového účtu USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  