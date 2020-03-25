---
title: DLP politika tipy nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932601"
---
# <a name="dlp-policy-tip-issues"></a>Problémy s tipmi politiky DLP

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

**Tipy pre politiku DLP**

Pri používaní **politík DLP**môžu byť používatelia upozornení na porušenie pravidiel pomocou **tipov politiky**. Správcovia môžu nakonfigurovať politiky tipy na zobrazenie pri testovaní ich DLP politiky alebo keď politika je v režime úplného výkonu.
  
Ak chcete konfigurovať tipy politiky v politike DLP v centre zabezpečenia a súladu v úplnom režime výkonu, postupujte nasledovne:
  
- Uistite sa, že politiky tipy boli **povolené** na DLP pravidlo pomocou krokov [tu](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Uistite sa, že váš **obsah zodpovedá** tomu, čo je **potrebné** na spustenie pravidla načrtnutého v tomto článku [tu](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Politika tipy Zobraziť v OWA a Outlook. Avšak, pri používaní **programu Outlook 2013 alebo novší**, politiky tipy sú zobrazené len za určitých podmienok. Tieto podmienky sú uvedené tu: [podporované podmienky pre program Outlook 2013 alebo novší pre zobrazenie politiky tipy](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Ďalšie informácie o tipy pre politiku DLP nájdete v téme: [Zobraziť tipy politiky pre politiky DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  