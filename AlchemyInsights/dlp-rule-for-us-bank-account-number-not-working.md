---
title: DLP pravidlo pre nás bankový účet číslo nefunguje
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
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389484"
---
Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **Číslo bankového účtu v USA** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre čo DLP politiky hľadá, keď sa vyhodnotí.
  
Napríklad, **Číslo bankového účtu v USA** politika nakonfigurovaná s 85% úrovni spoľahlivosti, takto hodnotia a musí zistiť pravidlo spustiť:
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 číslic

- **[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 číslic.

- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, neexistuje žiadny kontrolný súčet

- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politiky je 75% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:

  - Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru

  - Nájsť slovo od Keyword_usa_Bank_Account.

    Napríklad nasledujúca ukážka by spúšť pre politiky **USA číslo bankového účtu** : bežný účet 78344011

Pre viac informácií o čo je potrebné **Číslo bankového účtu v USA** sa vyhľadávajú pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií pozrite sa na číslo bankového účtu v USA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  