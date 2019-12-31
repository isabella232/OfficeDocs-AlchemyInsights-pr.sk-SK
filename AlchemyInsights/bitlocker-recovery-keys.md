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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="33e80-102">Prístup k kľúčom na obnovenie šifrovania BitLocker</span><span class="sxs-lookup"><span data-stu-id="33e80-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="33e80-103">Pri konfigurácii šifrovania BitLocker Nastavenie Endpoint Protection politiky, je možné definovať, či BitLocker obnovenie informácií by mali byť uložené v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33e80-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="33e80-104">Ak toto nastavenie je nakonfigurovaný, uložené údaje o obnovení by mali byť viditeľné pre správcu Intune ako súčasť údajov záznam zariadenia v zariadení Intune Blade dvoma spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="33e80-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="33e80-105">Zariadenia-Azure AD zariadenia-> "zariadenie" alebo zariadenia-> všetky zariadenia-> "Device"-> kľúče pre obnovenie</span><span class="sxs-lookup"><span data-stu-id="33e80-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="33e80-106">Prípadne, ak existuje správcovské prístup k zariadeniu samotného, kľúč na obnovenie (heslo) možno vidieť spustením nasledujúceho príkazu z príkazového riadka s právami správcu:</span><span class="sxs-lookup"><span data-stu-id="33e80-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="33e80-107">Ak bolo zariadenie šifrované pred zápisom do systému Intune, kľúč na obnovenie môže byť priradený k "kontu Microsoft" (MSA), ktoré sa používajú na prihlásenie do zariadenia počas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="33e80-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="33e80-108">Ak tomu tak bolo, prístup https://onedrive.live.com/recoverykey a prihlasovanie sa, že MSA by mal ukázať zariadenia, pre ktoré boli uložené kľúče na obnovenie.</span><span class="sxs-lookup"><span data-stu-id="33e80-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="33e80-109">Ak zariadenie bolo šifrované v dôsledku konfigurácie prostredníctvom doménovej skupinovej politiky, informácie o obnovení môžu byť uložené v on-premise služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33e80-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

