---
title: Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573531"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10

Základné údaje zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia. Základné údaje zabezpečenia sú predkonfigurované skupiny nastavení Windowsu, ktoré sa používajú na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia. Vytvorením základného profilu zabezpečenia v službe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadenia.

Keď nasadíte základné hodnoty zabezpečenia do skupín používateľov alebo zariadení, nastavenia sa použijú na zariadenia spustené vo Windowse 10 alebo novšom. Napríklad funkcia MDM Security Baseline automaticky (1) zapne funkciu BitLocker for vymeniteľných jednotiek, (2) vyžaduje heslo na odomknutie zariadenia a (3) zakáže základné overovanie. Ak predvolená hodnota v prostredí nie je funkčná, prispôsobte základnú čiaru tak, aby sa aplikovali potrebné nastavenia.

Základné informácie o zabezpečení tiež pomáhajú pri vytváraní pracovného postupu koncového zabezpečenia v programe Microsoft 365. Nižšie sú uvedené niektoré výhody tohto:

- Základná hodnota zabezpečenia obsahuje najvhodnejšie postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie. Keďže partneri služby Intune s tímom zabezpečenia systému Windows, ktorý vytvára základné hodnoty pre politiky skupiny, sú tieto odporúčania založené na solídnom poradenstve a rozsiahlych skúsenostiach.
- Ak sa v službe Intune nachádzate a neviete, kde začať, základné informácie o zabezpečení vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.
- Ak v súčasnosti používate skupinovú politiku, migrácia do služby Intune na účely správy je oveľa jednoduchšia so základmi zabezpečenia, pretože sú zabudované do služby Intune a obsahujú najmodernejšie možnosti spravovania.

Ďalšie informácie nájdete v téme [základné informácie o zabezpečení systému Windows](https://go.microsoft.com/fwlink/?linkid=2141503) a [Správa mobilných zariadení](https://go.microsoft.com/fwlink/?linkid=2141701).