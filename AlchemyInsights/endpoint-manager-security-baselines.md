---
title: EndPoint Manager – základné úrovne zabezpečenia
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
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923569"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – základné úrovne zabezpečenia

Základné úrovne zabezpečenia sú vopred nakonfigurované skupiny nastavení Windowsu, ktoré vám pomôžu použiť nastavenia zabezpečenia odporúčané príslušnými bezpečnostnými tímami. Tieto základné úrovne je možné prispôsobiť tak, aby obsahovali iba požadované nastavenia a hodnoty. Ďalšie informácie o základných úrovniach zabezpečenia nájdete v téme [Použitie základných úrovní zabezpečenia na konfiguráciu zariadení s Windowsom 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

V súčasnosti existujú základné úrovne pre tieto produkty:

- Nastavenie zabezpečenia MDM systému Windows
- Zabezpečenie Microsoft Defender pre koncové body
- Microsoft Edge

Všetky základné úrovne sa pravidelne aktualizujú a vydávajú v prírastkových verziách. V každej verzii sa pridávajú alebo odstraňujú nastavenia z predchádzajúcej verzie, aby sa zabezpečilo, že základná úroveň spĺňa aktuálne pokyny. Konzola so základnými úrovňami zabezpečenia v Endpoint Security umožňuje porovnať rôzne verzie pomocou viditeľných zmien medzi verziami.

Pokyny na najefektívnejšiu zmenu nasadenej verzie základnej úrovne nájdete v téme [Spravovanie základných úrovní zabezpečenia v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Po nasadení základnej úrovne zabezpečenia môžete monitorovať stav nasadenia a skontrolovať nastavenia podľa jednotlivých zariadení.

Keďže pôvodné hodnoty zabezpečenia obsahujú veľa nastavení, je dôležité skontrolovať zmeny konfigurácie a vykonať testovanie, aby ste zabezpečili, že všetky nastavenia sú vhodné pre vaše zariadenia a potreby podniku.

**Poznámka:** Údaje zostáv pre základné úrovne sa môžu zobraziť až o 24 hodín od počiatočného nasadenia do zariadenia a až o 6 hodín v prípade ďalších aktualizácií. 

Najčastejšou príčinou nepoužitia nastavení základnej úrovne je to, že rovnaké nastavenie sa používa v inom profile. Tento scenár možno preskúmať pre konkrétne zariadenie tak, že ho vyberiete z uzla stavu zariadenia v profile základnej úrovne zabezpečenia. Podrobnosti nájdete v téme [Riešenie konfliktov základných úrovní zabezpečenia](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).