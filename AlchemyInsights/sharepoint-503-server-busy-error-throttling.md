---
title: SharePoint Online obmedzovanie
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931241"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online obmedzovanie

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

**503 server je zaneprázdnený chyba**

Používatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive. 

Táto chyba môže byť spôsobená škrtenia v službe SharePoint. SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online. Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov. 

Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, či je aktívna údržba, ktorá sa vyskytuje na nájomníkovi, a to tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).

 Nakoniec, uistite sa, že navštívite stránku [služby zdravie](https://portal.office.com/adminportal/home#/servicehealth) skontrolovať všetky upozornenia/incidenty, ktoré môžu byť vyskytujúce.

