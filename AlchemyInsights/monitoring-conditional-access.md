---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713733"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="6169b-102">Monitorovanie podmieneného prístupu pre Exchange</span><span class="sxs-lookup"><span data-stu-id="6169b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="6169b-103">Používatelia zacielené na podmienený prístup dostanú e-mailové upozornenie, ak nespĺňajú požiadavky vašej organizácie na prístup.</span><span class="sxs-lookup"><span data-stu-id="6169b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6169b-104">Ak chcete vyriešiť, odporúčame jedno alebo viaceré z nasledujúcich riešení:</span><span class="sxs-lookup"><span data-stu-id="6169b-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="6169b-105">Ak sa predpokladá, že zariadenie je zapísané, radí používateľovi prejsť na firemný portál aplikácie a overiť, že sa zobrazí na portáli spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="6169b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6169b-106">Ak sa tak nestane, používateľ by mal zariadenie zapísať.</span><span class="sxs-lookup"><span data-stu-id="6169b-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="6169b-107">V Azure portál prejdite na **zariadenie Intune \> súlad zariadenia**.</span><span class="sxs-lookup"><span data-stu-id="6169b-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6169b-108">V časti **Monitor** kliknite na položku **zhoda zariadení**.</span><span class="sxs-lookup"><span data-stu-id="6169b-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="6169b-109">Zobrazte zostavu súladu so zariadením a overte, či je zariadenie používateľa označené ako vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="6169b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="6169b-110">V Azure portál prejdite na **zariadenie Intune \> súlad zariadenia**.</span><span class="sxs-lookup"><span data-stu-id="6169b-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6169b-111">V časti **Spravovať**kliknite na položku **politiky**.</span><span class="sxs-lookup"><span data-stu-id="6169b-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="6169b-112">V zozname politík súladu overte, či je profil priradený zariadeniu používateľa.</span><span class="sxs-lookup"><span data-stu-id="6169b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6169b-113">Ak nie je priradený žiadny profil, Intune nebude môcť potvrdiť stav súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="6169b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="6169b-114">Upravte priradenie podmieneného prístupu používateľa.</span><span class="sxs-lookup"><span data-stu-id="6169b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="6169b-115">V Azure portál prejsť na **Intune \> podmieneného prístupu \> politiky**</span><span class="sxs-lookup"><span data-stu-id="6169b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="6169b-116">Vybrať politiku zo zoznamu</span><span class="sxs-lookup"><span data-stu-id="6169b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="6169b-117">Kliknite na položku **Používatelia a skupiny**</span><span class="sxs-lookup"><span data-stu-id="6169b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="6169b-118">Ak chcete zacieliť určitú politiku na niekoho, pridajte ich do zoznamu **zahrnúť** .</span><span class="sxs-lookup"><span data-stu-id="6169b-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="6169b-119">Ak chcete zabezpečiť, aby bola osoba vynechaná z politiky, pridajte ich do zoznamu **výnimiek** .</span><span class="sxs-lookup"><span data-stu-id="6169b-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="6169b-120">Čítajte viac: [ako sledovať zariadenia podmieneného prístupu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="6169b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

