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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505083"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="c1351-102">Prístup ku kľúčem na obnovenie pre šifrovanie BitLocker</span><span class="sxs-lookup"><span data-stu-id="c1351-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="c1351-103">Pri konfigurácii nastavení šifrovania BitLocker Politika ochrany koncových bodov služby Intune je možné definovať, či sa majú informácie o obnove pre šifrovanie BitLocker uložiť do služby Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1351-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="c1351-104">Ak je toto nastavenie nakonfigurované, uložené údaje o obnove by mal vidieť správca služby Intune ako súčasť údajov záznamu zariadenia v zariadeniach Intune blade dvoma spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="c1351-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="c1351-105">Zariadenia – zariadenia so službou Azure AD > zariadenie alebo zariadenia –> všetky zariadenia -> "zariadenie" > kľúče na obnovenie</span><span class="sxs-lookup"><span data-stu-id="c1351-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="c1351-106">Prípadne, ak existuje správcovský prístup k samotnému zariadeniu, kľúč na obnovenie (Heslo) je možné zobraziť spustením nasledujúceho príkazu v príkazovom riadku bez oprávnení:</span><span class="sxs-lookup"><span data-stu-id="c1351-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="c1351-107">Ak bolo zariadenie zašifrované pred zaregistrovaním do služby Intune, kľúč na obnovenie možno bol priradený ku kontu Microsoft (MSA), ktoré sa používa na prihlásenie do zariadenia počas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="c1351-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="c1351-108">V takom prípade by sa pri prístupe k msA a prihlásení s týmto zariadením mali zobraziť zariadenia, pre ktoré boli uložené  https://onedrive.live.com/recoverykey kľúče na obnovenie.</span><span class="sxs-lookup"><span data-stu-id="c1351-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="c1351-109">Ak bolo zariadenie zašifrované v dôsledku konfigurácie prostredníctvom skupinovej politiky založenej na doméne, informácie o obnove môžu byť uložené v presnej službe Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1351-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="c1351-110">Ak ste nakonfigurovali politiku ochrany koncového bodu na ukladanie kľúča na obnovenie v službe Azure Active Directory, ale kľúč pre konkrétne zariadenie nebol nahraný, nahrávanie môžete spustiť otočením kľúča na obnovenie pre toto zariadenie z konzoly MEM.</span><span class="sxs-lookup"><span data-stu-id="c1351-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="c1351-111">Podrobnosti nájdete v téme [Otočenie kľúčov na obnovenie pre šifrovanie BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="c1351-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

