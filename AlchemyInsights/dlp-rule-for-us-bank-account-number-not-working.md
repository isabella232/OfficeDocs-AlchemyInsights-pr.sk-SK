---
title: DLP pravidlo pre číslo bankového účtu v USA nefunguje
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005033"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problémy S DLP číslami bankových kont v USA

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy S DLP číslami bankových kont v USA**

Máte problémy s ochrana pred stratou údajov **(DLP)** v obsahu obsahujúcom číslo bankového účtu **v** USA pri používaní citlivých informácií typu DLP v O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá pri vyhodnocovaní.
  
Napríklad pre politiku čísla bankového účtu **v** USA nakonfigurovanej na úrovni spoľahlivosti 85 % sa vyhodnotí nasledovné a musí sa zistiť, aby sa toto pravidlo spustilo:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8 – 17 číslic

- **[Vzorka:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 – 17 po sebe idúcich číslic

- **[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii

- **[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Politika DLP si je na 75% istá, že sa zistil tento typ citlivej informácie, ak v blízkosti 300 znakov:

  - Výraz výrazu Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru

  - Nájde sa kľúčové Keyword_usa_Bank_Account kľúčové slovo z tejto lokality.

    Napríklad nasledujúca ukážka by spustila politiku **Číslo bankového účtu v USA:** Checking Account 78344011

Ďalšie informácie o tom,  čo sa vyžaduje na to, aby sa zistilo číslo vášho obsahu bankového účtu v USA, nájdete v nasledujúcej časti tohto článku: Čo typy citlivých informácií vyžadujú číslo bankového účtu v [USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Ak používate iný vstavaný typ citlivých informácií, informácie potrebné pre iné typy informácií nájdete v nasledujúcom článku: Čo [typy citlivých informácií hľadať](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  