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
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538785"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="1ce13-102">Monitorovanie podmieneného prístupu pre výmenu</span><span class="sxs-lookup"><span data-stu-id="1ce13-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="1ce13-103">Užívatelia cielené s podmieneným prístupom dostane e-mail s upozornením, ak nespĺňajú požiadavky vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="1ce13-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="1ce13-104">Ak chcete vyriešiť, odporúčame jeden alebo viac z nasledujúcich riešení:</span><span class="sxs-lookup"><span data-stu-id="1ce13-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="1ce13-105">Ak zariadenie predpokladá sa zapísal, poradiť užívateľovi ísť k aplikácie portáli spoločnosti a overte, že sa zdá, na portáli spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="1ce13-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="1ce13-106">Ak to tak nie je, používateľ by mal zapísať zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1ce13-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="1ce13-107">Na portáli Azure ísť do **Intune \> zariadenia súlad**.</span><span class="sxs-lookup"><span data-stu-id="1ce13-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1ce13-108">Pod **monitorom s** kliknite na **zariadenie súladu**.</span><span class="sxs-lookup"><span data-stu-id="1ce13-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="1ce13-109">Zobrazenia zostavy súladu zariadení na overenie, že zariadenie používateľa je označená ako vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="1ce13-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="1ce13-110">Na portáli Azure ísť do **Intune \> zariadenia súlad**.</span><span class="sxs-lookup"><span data-stu-id="1ce13-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1ce13-111">Podľa **Spravovať**, kliknite na položku **politiky**.</span><span class="sxs-lookup"><span data-stu-id="1ce13-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="1ce13-112">V zozname súladu politík, overiť, že profil je priradený k zariadení vášho používateľa.</span><span class="sxs-lookup"><span data-stu-id="1ce13-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1ce13-113">Ak je priradený žiadny profil, potom Intune nebude schopný potvrdiť zhodu stav zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1ce13-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="1ce13-114">Upraviť priradenie podmieneného prístupu.</span><span class="sxs-lookup"><span data-stu-id="1ce13-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="1ce13-115">Na portáli Azure ísť do **Intune \> podmieneného prístupu \> podmienky**</span><span class="sxs-lookup"><span data-stu-id="1ce13-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="1ce13-116">Zo zoznamu vyberte politiku</span><span class="sxs-lookup"><span data-stu-id="1ce13-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="1ce13-117">Kliknite na tlačidlo **používateľov a skupín**</span><span class="sxs-lookup"><span data-stu-id="1ce13-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="1ce13-118">Osloviť určitú politiku na niekoho pridať do zoznamu pre **zahrnutie** .</span><span class="sxs-lookup"><span data-stu-id="1ce13-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="1ce13-119">Zabezpečiť, že osoba je vynechaný z politiky, pridajte ich do zoznamu **vylúčenie** .</span><span class="sxs-lookup"><span data-stu-id="1ce13-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="1ce13-120">Prečítajte si viac: [ako Monitor podmieneného prístupu zariadenia](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="1ce13-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

