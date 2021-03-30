---
title: EndPoint Manager – pôvodné hodnoty zabezpečenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421090"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – pôvodné hodnoty zabezpečenia

Pôvodné hodnoty zabezpečenia sú vopred nakonfigurované skupiny nastavení Windowsu, ktoré vám pomôžu použiť nastavenia zabezpečenia odporúčané príslušnými tímami zabezpečenia. Tieto pôvodné hodnoty je možné prispôsobiť tak, aby sa doručovali iba požadované nastavenia a hodnoty. Ďalšie informácie o pôvodných plánoch zabezpečenia nájdete v téme [Použitie pôvodných bodov zabezpečenia na konfiguráciu zariadení s Windowsom 10 v intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Pre tieto produkty v súčasnosti existujú pôvodné hodnoty:

- Nastavenia zabezpečenia MDM systému Windows
- Zabezpečenie aplikácie Microsoft Defender pre EndPoint
- Microsoft Edge

Všetky pôvodné hodnoty sa pravidelne aktualizujú a uvoľňujú v prírastkových verziách. Každá verzia pridá alebo odstráni nastavenia z predchádzajúcej verzie, aby sa zabezpečilo, že základná čiara spĺňa aktuálne pokyny. Konzola s pôvodnými plánmi zabezpečenia v časti Zabezpečenie koncového bodu umožňuje porovnanie rôznych verzií tak, že zmeny z verzie na verziu sa zobrazia.

Pokyny na najefektívnejšie zmeny toho, ktorá verzia pôvodného plánu je nasadená, nájdete v téme Správa profilov pôvodného plánu zabezpečenia [v Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Po nasadení základnej hodnoty zabezpečenia môžete sledovať stav nasadenia a skontrolovať nastavenia na každom zariadení.

**Poznámka:** Vykazovanie údajov pre pôvodné hodnoty môže trvať až 24 hodín, kým sa zobrazia od prvého nasadenia do zariadenia, a až 6 hodín pre ďalšie aktualizácie. 

Najčastejšou príčinou, prečo sa nastavenie pôvodného plánu nepoužíva, je to, že rovnaké nastavenie sa používa v inom profile. Tento scenár môžete preskúmať pre konkrétne zariadenie tak, že toto zariadenie vyberiete z uzla Stav zariadenia v profile Plán zabezpečenia. Podrobnosti nájdete v téme [Riešenie konfliktov pre pôvodné hodnoty zabezpečenia.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)