---
title: DLP pravidlo číslo kreditnej karty nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919095"
---
Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúcich **Čísla kreditnej karty** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre spustenie DLP politiky, keď sa vyhodnotí. Napríklad pre **kreditnú kartu politiky** nakonfigurované s 85% úrovni spoľahlivosti, takto hodnotia a musí zistiť pravidlo spustiť: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môže byť formátovaný alebo neformátovaný (dddddddddddddddd) a musí vyhovieť skúške Luhn. 
    
- **[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi komplexný a robustný vzor, ktorý detekuje karty od všetkých významných značiek po celom svete, vrátane Visa, Mastercard, Discover Card, JCB, American Express, darčekové poukážky a karty stravník. 
    
- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný 
    
- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politiky je 85% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov: 
    
  - Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.
    
  - Je splnená jedna z nasledujúcich možností: 
    
  - Nájsť slovo od Keyword_cc_verification.
    
  - Kľúčové slovo z Keyword_cc_name nájdených
    
  - Funkcia Func_expiration_date zistí dátum správny dátum formát.
    
  - Kontrolný prechádza
    
    Napríklad nasledujúca ukážka by spúšť pre DLP politika číslo kreditnej karty:
    
  - Víza: 4485 3647 3952 7352 
    
  - Platnosť: 2/2009
    
Pre viac informácií o čo je nevyhnutné pre **Číslo kreditnej karty** je možné pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií vyhľadajte kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

