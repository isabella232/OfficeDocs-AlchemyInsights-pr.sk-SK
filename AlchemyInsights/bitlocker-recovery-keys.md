---
title: Kľúče na obnovenie pre šifrovanie BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060079"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prístup ku kľúčem na obnovenie pre šifrovanie BitLocker

Pri konfigurácii nastavení šifrovania BitLocker Politika ochrany koncových bodov služby Intune je možné definovať, či sa majú informácie o obnove pre šifrovanie BitLocker ukladať Azure Active Directory.

Ak je toto nastavenie nakonfigurované, uložené údaje o obnove by mal vidieť správca služby Intune ako súčasť údajov záznamu zariadenia v zariadeniach Intune blade dvoma spôsobmi:

Zariadenia – zariadenia so službou Azure AD > zariadenie alebo zariadenia –> všetky zariadenia -> "zariadenie" > kľúče na obnovenie

Prípadne, ak existuje správcovský prístup k samotnému zariadeniu, kľúč na obnovenie (Heslo) je možné zobraziť spustením nasledujúceho príkazu v príkazovom riadku bez oprávnení:

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
Ak bolo zariadenie zašifrované pred zaregistrovaním do služby Intune, kľúč na obnovenie možno bol priradený ku kontu Microsoft (MSA), ktoré sa používa na prihlásenie do zariadenia počas procesu OOBE. V takom prípade by sa pri prístupe k msA a prihlásení s týmto zariadením mali zobraziť zariadenia, pre ktoré boli uložené  https://onedrive.live.com/recoverykey kľúče na obnovenie.
 
Ak bolo zariadenie zašifrované v dôsledku konfigurácie prostredníctvom skupinovej politiky založenej na doméne, informácie o obnove môžu byť uložené v presnej službe Active Directory.

Ak ste nakonfigurovali politiku ochrany koncového bodu na ukladanie kľúča na obnovenie v balíku Azure Active Directory ale kľúč pre konkrétne zariadenie nebol nahraný, môžete spustiť nahrávanie otočením kľúča na obnovenie pre toto zariadenie z konzoly MEM. Podrobnosti nájdete v téme [Otočenie kľúčov na obnovenie pre šifrovanie BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

