---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708689"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="136e3-102">Monitorovanie podmieneného prístupu pre Exchange</span><span class="sxs-lookup"><span data-stu-id="136e3-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="136e3-103">Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="136e3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="136e3-104">Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:</span><span class="sxs-lookup"><span data-stu-id="136e3-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="136e3-105">Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli.</span><span class="sxs-lookup"><span data-stu-id="136e3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="136e3-106">Ak to tak nie je, používateľ by mal zariadenie zaregistrovať.</span><span class="sxs-lookup"><span data-stu-id="136e3-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="136e3-107">Na portáli Azure prejdite do služby Intune > súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="136e3-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="136e3-108">V časti monitor kliknite na položku súlad zariadenia.</span><span class="sxs-lookup"><span data-stu-id="136e3-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="136e3-109">Ak chcete overiť, či je zariadenie používateľa označené ako vyhovujúce, pozrite si zostavu súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="136e3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="136e3-110">Na portáli Azure prejdite do služby Intune > súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="136e3-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="136e3-111">V časti Spravovať kliknite na položku politiky.</span><span class="sxs-lookup"><span data-stu-id="136e3-111">Under Manage, click Policies.</span></span> <span data-ttu-id="136e3-112">V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa.</span><span class="sxs-lookup"><span data-stu-id="136e3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="136e3-113">Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="136e3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="136e3-114">Upravte priradenie podmieneného prístupu používateľa.</span><span class="sxs-lookup"><span data-stu-id="136e3-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="136e3-115">Na portáli Azure prejdite na   >  **politiky podmieneného prístupu** služby Intune  >  .</span><span class="sxs-lookup"><span data-stu-id="136e3-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="136e3-116">Zo zoznamu vyberte politiku.</span><span class="sxs-lookup"><span data-stu-id="136e3-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="136e3-117">Kliknite na položku Používatelia a skupiny.</span><span class="sxs-lookup"><span data-stu-id="136e3-117">Click Users and groups.</span></span>
4. <span data-ttu-id="136e3-118">Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do zoznamu zahrnúť.</span><span class="sxs-lookup"><span data-stu-id="136e3-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="136e3-119">Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do zoznamu výnimiek.</span><span class="sxs-lookup"><span data-stu-id="136e3-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="136e3-120">Užitočné prepojenia:</span><span class="sxs-lookup"><span data-stu-id="136e3-120">Helpful links:</span></span>

[<span data-ttu-id="136e3-121">Prehľad súladu zariadenia</span><span class="sxs-lookup"><span data-stu-id="136e3-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="136e3-122">Riešenie problémov s certifikačnou autoritou</span><span class="sxs-lookup"><span data-stu-id="136e3-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="136e3-123">Politika riešenia problémov</span><span class="sxs-lookup"><span data-stu-id="136e3-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="136e3-124">Sledovanie dodržiavania súladu zariadenia Intune</span><span class="sxs-lookup"><span data-stu-id="136e3-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="136e3-125">Poznámka: tieto kroky sú užitočné len pri riešení problémov s podmieneným prístupom funkcie Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="136e3-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="136e3-126">Je tiež možné do karantény zablokovať zariadenie, ktoré blokuje prístup k e-mailu pomocou politiky Exchange.</span><span class="sxs-lookup"><span data-stu-id="136e3-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="136e3-127">Ďalšie informácie o spravovaní zariadení s Exchangeom nájdete v téme [tu] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="136e3-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
