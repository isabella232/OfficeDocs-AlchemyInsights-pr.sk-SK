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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702918"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="8e261-102">Monitorovanie podmieneného prístupu pre Exchange</span><span class="sxs-lookup"><span data-stu-id="8e261-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="8e261-103">Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="8e261-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="8e261-104">Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:</span><span class="sxs-lookup"><span data-stu-id="8e261-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="8e261-105">Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli.</span><span class="sxs-lookup"><span data-stu-id="8e261-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="8e261-106">Ak to tak nie je, používateľ by mal zariadenie zaregistrovať.</span><span class="sxs-lookup"><span data-stu-id="8e261-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="8e261-107">Na portáli Azure prejdite na \*\* \> súlad zariadenia\*\*so službou Intune.</span><span class="sxs-lookup"><span data-stu-id="8e261-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8e261-108">V časti **Monitor** kliknite na položku **súlad zariadenia**.</span><span class="sxs-lookup"><span data-stu-id="8e261-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="8e261-109">Ak chcete overiť, či je zariadenie používateľa označené ako vyhovujúce, pozrite si zostavu súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8e261-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="8e261-110">Na portáli Azure prejdite na \*\* \> súlad zariadenia\*\*so službou Intune.</span><span class="sxs-lookup"><span data-stu-id="8e261-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8e261-111">V časti **Spravovať**kliknite na položku **politiky**.</span><span class="sxs-lookup"><span data-stu-id="8e261-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="8e261-112">V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa.</span><span class="sxs-lookup"><span data-stu-id="8e261-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="8e261-113">Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8e261-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="8e261-114">Upravte priradenie podmieneného prístupu používateľa.</span><span class="sxs-lookup"><span data-stu-id="8e261-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="8e261-115">Na portáli Azure prejdite na \*\* \> \> politiky podmieneného prístupu služby Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="8e261-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="8e261-116">Výber politiky v zozname</span><span class="sxs-lookup"><span data-stu-id="8e261-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="8e261-117">Kliknite na položku **Používatelia a skupiny**</span><span class="sxs-lookup"><span data-stu-id="8e261-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="8e261-118">Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do zoznamu **zahrnúť** .</span><span class="sxs-lookup"><span data-stu-id="8e261-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="8e261-119">Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do zoznamu **výnimiek** .</span><span class="sxs-lookup"><span data-stu-id="8e261-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="8e261-120">Ďalšie informácie: [ako sledovať zariadenia s podmieneným prístupom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="8e261-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

