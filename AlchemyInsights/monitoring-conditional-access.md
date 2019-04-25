---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418484"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="21227-102">Monitorovanie podmieneného prístupu</span><span class="sxs-lookup"><span data-stu-id="21227-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="21227-103">Užívatelia cielené s podmieneným prístupom dostane e-mail s upozornením, ak nespĺňajú požiadavky vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="21227-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="21227-104">Ak chcete vyriešiť, odporúčame jeden alebo viac z nasledujúcich riešení:</span><span class="sxs-lookup"><span data-stu-id="21227-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="21227-105">Ak zariadenie predpokladá sa zapísal, poradiť užívateľovi ísť k aplikácie portáli spoločnosti a overte, že sa zdá, na portáli spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="21227-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="21227-106">Ak to tak nie je, používateľ by mal zapísať zariadenia.</span><span class="sxs-lookup"><span data-stu-id="21227-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="21227-107">Na portáli Azure ísť do **Intune \> zariadenia súlad**.</span><span class="sxs-lookup"><span data-stu-id="21227-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="21227-108">Pod **monitorom s** kliknite na **zariadenie súladu**.</span><span class="sxs-lookup"><span data-stu-id="21227-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="21227-109">Zobrazenia zostavy súladu zariadení na overenie, že zariadenie používateľa je označená ako vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="21227-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="21227-110">Na portáli Azure ísť do **Intune \> zariadenia súlad**.</span><span class="sxs-lookup"><span data-stu-id="21227-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="21227-111">Podľa **Spravovať**, kliknite na položku **politiky**.</span><span class="sxs-lookup"><span data-stu-id="21227-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="21227-112">V zozname súladu politík, overiť, že profil je priradený k zariadení vášho používateľa.</span><span class="sxs-lookup"><span data-stu-id="21227-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="21227-113">Ak je priradený žiadny profil, potom Intune nebude schopný potvrdiť zhodu stav zariadenia.</span><span class="sxs-lookup"><span data-stu-id="21227-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="21227-114">Upraviť priradenie podmieneného prístupu.</span><span class="sxs-lookup"><span data-stu-id="21227-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="21227-115">Na portáli Azure ísť do **Intune \> podmieneného prístupu \> podmienky**</span><span class="sxs-lookup"><span data-stu-id="21227-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="21227-116">Zo zoznamu vyberte politiku</span><span class="sxs-lookup"><span data-stu-id="21227-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="21227-117">Kliknite na tlačidlo **používateľov a skupín**</span><span class="sxs-lookup"><span data-stu-id="21227-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="21227-118">Osloviť určitú politiku na niekoho pridať do zoznamu pre **zahrnutie** .</span><span class="sxs-lookup"><span data-stu-id="21227-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="21227-119">Zabezpečiť, že osoba je vynechaný z politiky, pridajte ich do zoznamu **vylúčenie** .</span><span class="sxs-lookup"><span data-stu-id="21227-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="21227-120">Prečítajte si viac: [ako Monitor podmieneného prístupu zariadenia](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="21227-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

