---
title: Inventár softvéru chýba alebo je nepresný
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676514"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="9219b-102">Inventár softvéru chýba alebo je nepresný</span><span class="sxs-lookup"><span data-stu-id="9219b-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="9219b-103">Inventár softvéru v Spravovanie hrozieb a rizík (TVM) je zoznam známeho softvéru vo vašej organizácii s oficiálnymi bežnými enumeráciami platformy (CPE).</span><span class="sxs-lookup"><span data-stu-id="9219b-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="9219b-104">Softvérové produkty bez oficiálneho CPE nemajú publikované slabé miesta.</span><span class="sxs-lookup"><span data-stu-id="9219b-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="9219b-105">Inventár obsahuje aj podrobnosti, ako je napríklad názov dodávateľa, počet ľudí, hrozby a počet odovených zariadení.</span><span class="sxs-lookup"><span data-stu-id="9219b-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="9219b-106">Zmeny softvéru v zariadeniach sa zvyčajne prejavia na portáloch zabezpečenia do dvoch hodín.</span><span class="sxs-lookup"><span data-stu-id="9219b-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="9219b-107">Niekedy však môže trvať dlhšie.</span><span class="sxs-lookup"><span data-stu-id="9219b-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="9219b-108">Momentálne nie je možné vynútiť synchronizáciu. toto je priebežné priebežné hodnotenie.</span><span class="sxs-lookup"><span data-stu-id="9219b-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="9219b-109">Ak ste vykonali zmenu softvéru a po 5 hodinách sa zmena v TVM neprejaví presne, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="9219b-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="9219b-110">Skontrolujte časť s dôkazmi o softvéri a porozumiete tomu, ako sa softvér zistil.</span><span class="sxs-lookup"><span data-stu-id="9219b-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="9219b-111">Uistite sa, že softvér je podporovaný.</span><span class="sxs-lookup"><span data-stu-id="9219b-111">Make sure that the software is supported.</span></span> <span data-ttu-id="9219b-112">Softvér sa môže zobrazovať iba na úrovni zariadenia aj vtedy, ak ho v súčasnosti nepodporuje Spravovanie hrozieb a rizík.</span><span class="sxs-lookup"><span data-stu-id="9219b-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="9219b-113">K dispozícii sú však len obmedzené údaje.</span><span class="sxs-lookup"><span data-stu-id="9219b-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="9219b-114">Kroky na nahlásenie nepresnosti z portálu nájdete v téme [Nepresná zostava.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="9219b-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="9219b-115">**Poznámka:** Hlásenie nepresných údajov z portálu MDE je jednosmerný kanál pre inžinierov.</span><span class="sxs-lookup"><span data-stu-id="9219b-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="9219b-116">Ak ide o súrny problém, otvorte tiket technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="9219b-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="9219b-117">Ďalšie informácie nájdete v téme [Inventár softvéru – Spravovanie hrozieb a rizík.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="9219b-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>