---
title: Kľúče na obnovenie pre šifrovanie BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685901"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prístup k kľúčom na obnovenie šifrovania BitLocker

Pri konfigurácii politiky ochrany koncového bodu služby BitLocker Settings Intune je možné určiť, či sa majú informácie o obnovení šifrovania BitLocker uložiť v službe Azure Active Directory.

Ak je toto nastavenie nakonfigurované, uložené údaje obnovenia by sa mali zobraziť správcovi služby Intune ako súčasť údajov v záznamoch zariadenia v nástrojoch Intune, a to dvomi spôsobmi:

Zariadenia – Azure reklamné zariadenia – > "zariadenie" alebo zariadenia – > všetky zariadenia – > "zariadenie" – > kľúče na obnovenie

Prípadne, ak je správcovský prístup k samotnému zariadeniu, kľúč na obnovenie (heslo) je možné zobraziť spustením nasledujúceho príkazu z príkazového riadka s právami správcu:

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
Ak bolo zariadenie pred zadaním do služby Intune šifrované, kľúč na obnovenie sa mohol priradiť k kontu Microsoft (MSA), ktoré sa používa na prihlásenie do zariadenia počas procesu OOBE. Ak tomu tak bolo, prístup  https://onedrive.live.com/recoverykey a prihlasovanie pomocou tohto nástroja MSA by malo zobraziť zariadenia, pre ktoré boli kľúče obnovenia uložené.
 
Ak bolo zariadenie zašifrované ako dôsledok konfigurácie prostredníctvom skupinovej politiky založenej na doméne, informácie o obnovení sa môžu uložiť v lokálnom adresári služby Active Directory.
 

