---
title: DLP môže potrebovať vlastný typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932673"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP môže potrebovať vlastný typ

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

**DLP môže vyžadovať typ vlastného informácie**

Pomocou politiky ochrany pred únikom údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo vašej organizácii. V niektorých prípadoch môže byť potrebné **vytvoriť vlastný typ citlivých informácií** na ochranu údajov organizácie.

Vaša organizácia môže napríklad potrebovať identifikovať a chrániť identifikátory zamestnancov alebo iné údaje v určitom formáte špecifickom pre vašu organizáciu. Ak áno, pozrite si nasledujúce články pre viac informácií.
  
 **Prispôsobenie vstavaného typu citlivých informácií**
  
Ak by vstavaný typ citlivých informácií spĺňal vaše potreby len s niekoľkými vylepšeniami, môžete [prispôsobiť vstavaný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.
  
 **Vytvorenie vlastného typu citlivých informácií**
  
Ak však potrebujete úplne identifikovať a ochrániť iný typ citlivých informácií, môžete [vytvoriť vlastný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v používateľskom rozhraní centra zabezpečenia & Compliance Center.
  
**Vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell**

Nakoniec, ak UI neposkytuje všetky možnosti, ktoré potrebujete, môžete [vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Spustením súboru XML môžete použiť každú dostupnú možnosť.
