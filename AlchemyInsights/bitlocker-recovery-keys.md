---
title: Kľúče na obnovenie šifrovania BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908829"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prístup k kľúčom na obnovenie šifrovania BitLocker

Pri konfigurácii šifrovania BitLocker Nastavenie Endpoint Protection politiky, je možné definovať, či BitLocker obnovenie informácií by mali byť uložené v Azure Active Directory.

Ak toto nastavenie je nakonfigurovaný, uložené údaje o obnovení by mali byť viditeľné pre správcu Intune ako súčasť údajov záznam zariadenia v zariadení Intune Blade dvoma spôsobmi:

Zariadenia-Azure AD zariadenia-> "zariadenie" alebo zariadenia-> všetky zariadenia-> "Device"-> kľúče pre obnovenie

Prípadne, ak existuje správcovské prístup k zariadeniu samotného, kľúč na obnovenie (heslo) možno vidieť spustením nasledujúceho príkazu z príkazového riadka s právami správcu:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ak bolo zariadenie šifrované pred zápisom do systému Intune, kľúč na obnovenie môže byť priradený k "kontu Microsoft" (MSA), ktoré sa používajú na prihlásenie do zariadenia počas procesu OOBE. Ak tomu tak bolo, prístup https://onedrive.live.com/recoverykey a prihlasovanie sa, že MSA by mal ukázať zariadenia, pre ktoré boli uložené kľúče na obnovenie.
 
Ak zariadenie bolo šifrované v dôsledku konfigurácie prostredníctvom doménovej skupinovej politiky, informácie o obnovení môžu byť uložené v on-premise služby Active Directory.
 

