---
title: Politika ochrany aplikácií
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423961"
---
# <a name="application-protection-policy"></a><span data-ttu-id="3e54f-102">Politika ochrany aplikácií</span><span class="sxs-lookup"><span data-stu-id="3e54f-102">Application protection policy</span></span>

<span data-ttu-id="3e54f-103">Ak ste novým problémom s politikou ochrany aplikácií (APP), pozrite si prehľad [politík ochrany aplikácií](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="3e54f-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="3e54f-104">Ak chcete začať používať aplikáciu, pozrite si [tému Vytvorenie a priradenie politík ochrany aplikácií](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="3e54f-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="3e54f-105">Požiadavky politiky ochrany aplikácií:</span><span class="sxs-lookup"><span data-stu-id="3e54f-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="3e54f-106">Používateľ má licenciu Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="3e54f-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="3e54f-107">Používateľ patrí do skupiny zacielenej politikami ochrany aplikácií.</span><span class="sxs-lookup"><span data-stu-id="3e54f-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="3e54f-108">Do chránených aplikácií v zariadení je prihlásený iba jeden podnikový používateľ.</span><span class="sxs-lookup"><span data-stu-id="3e54f-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="3e54f-109">Aplikácia implementovala [Súpravu Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="3e54f-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="3e54f-110">Zoznam aplikácií, ktoré podporujú súpravu SDK, nájdete v téme Chránené aplikácie služby [Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="3e54f-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="3e54f-111">Politiky platia po tom, ako sa používateľ, ktorý spĺňa vyššie uvedené požiadavky, prihlási do aplikácie s podporou súpravy Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="3e54f-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="3e54f-112">Najjednoduchším spôsobom, ako zistiť, či sa použije politika, je požadovať, aby používateľ nastaviť pripnutie v politike.</span><span class="sxs-lookup"><span data-stu-id="3e54f-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="3e54f-113">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="3e54f-113">For more information, see:</span></span>

[<span data-ttu-id="3e54f-114">Najčastejšie otázky o riešení problémov s APP/MAM</span><span class="sxs-lookup"><span data-stu-id="3e54f-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="3e54f-115">Overenie nastavenia politiky ochrany aplikácií</span><span class="sxs-lookup"><span data-stu-id="3e54f-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="3e54f-116">Informácie o časovaní doručenia zásad ochrany aplikácií</span><span class="sxs-lookup"><span data-stu-id="3e54f-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="3e54f-117">Ako sledovať politiky ochrany aplikácií</span><span class="sxs-lookup"><span data-stu-id="3e54f-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)