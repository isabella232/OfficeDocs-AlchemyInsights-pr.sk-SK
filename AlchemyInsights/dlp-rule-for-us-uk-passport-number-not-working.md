---
title: DLP pravidlo pre USA / UK číslo pasu nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786713"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP - USA / UK čísla pasov

Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **USA / číslo pasu Spojeného kráľovstva** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre čo DLP politiky hľadá, keď sa vyhodnotí. 
  
Napríklad pre **USA / číslo pasu Spojeného kráľovstva** politika nakonfigurovaná s hrdosťou úroveň 75%, tieto sa vyhodnocujú a musí byť zistené pravidla vyvolať 
  
- **[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deväť číslic 
    
- **[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deväť po sebe idúcich číslic 
    
- **[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, neexistuje žiadny kontrolný súčet 
    
- **[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politiky je 75% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov: 
    
  - Funkcia Func_usa_uk_passport nájde obsah, ktorý zodpovedá vzoru.
    
  - Nájsť slovo od Keyword_passport.
    
    Napríklad nasledujúca ukážka by spúšť pre **USA / číslo pasu Spojeného kráľovstva** politiky: pas USA číslo 123456789 
    
Pre viac informácií o čo je nevyhnutné pre USA / UK pasové údaje sa vyhľadávajú pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [čo citlivé druhy informácií vzhľad pre USA / číslo pasu Spojeného kráľovstva](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

