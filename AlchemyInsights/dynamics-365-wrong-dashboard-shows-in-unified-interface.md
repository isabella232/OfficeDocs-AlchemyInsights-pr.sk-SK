---
title: Dynamics 365-nesprávne Dashboard relácie v Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528566"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="855c4-102">Nesprávne Dashboard relácie v Dynamics 365 zjednotené rozhranie</span><span class="sxs-lookup"><span data-stu-id="855c4-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="855c4-103">Existuje niekoľko dôvodov, prečo sa môže zobraziť iná tabuľa ako tá, ktorú očakávate:</span><span class="sxs-lookup"><span data-stu-id="855c4-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="855c4-104">Používateľ nastaviť predvolenú tabuľu používateľa</span><span class="sxs-lookup"><span data-stu-id="855c4-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="855c4-105">Zvyčajne môžete identifikovať predvolenú tabuľu používateľa je nastavená, ak tlačidlo **nastaviť ako predvolené** nezobrazuje v paneli príkazov tabule.</span><span class="sxs-lookup"><span data-stu-id="855c4-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="855c4-106">Predvolená tabuľa používateľa prepíše všetky ostatné predvolené tabule, a to aj v prípade, že predvolená tabuľa používateľa nie je v aktuálnej aplikácii.</span><span class="sxs-lookup"><span data-stu-id="855c4-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="855c4-107">Ak chcete zrušiť nastavenie predvolenej tabule, použite nasledujúce riešenie.</span><span class="sxs-lookup"><span data-stu-id="855c4-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="855c4-108">Vytvorte novú osobnú tabuľu.</span><span class="sxs-lookup"><span data-stu-id="855c4-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="855c4-109">Nastaví novú tabuľu ako predvolenú používateľa.</span><span class="sxs-lookup"><span data-stu-id="855c4-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="855c4-110">Odstrániť túto tabuľu.</span><span class="sxs-lookup"><span data-stu-id="855c4-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="855c4-111">Tabuľa je nastavená v Sitemap</span><span class="sxs-lookup"><span data-stu-id="855c4-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="855c4-112">Možno ste nastavili predvolenú tabuľu organizácie výberom tabule a výberom položky "nastaviť ako predvolené" v časti Prispôsobenie systému.</span><span class="sxs-lookup"><span data-stu-id="855c4-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="855c4-113">Ale Dashboard definované v Sitemap Designer bude mať prednosť pred tejto tabuli, ak má používateľ prístup k nemu.</span><span class="sxs-lookup"><span data-stu-id="855c4-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="855c4-114">Ak chcete, aby používatelia videli tabuľu, ktorú ste nastavili ako predvolenú organizáciu, môžete buď:</span><span class="sxs-lookup"><span data-stu-id="855c4-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="855c4-115">Nastaviť, že tabuľa v Sitemap</span><span class="sxs-lookup"><span data-stu-id="855c4-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="855c4-116">Odstránenie prístupu k Sitemap definované Dashboard pre týchto používateľov</span><span class="sxs-lookup"><span data-stu-id="855c4-116">Remove access to the sitemap defined dashboard for those users</span></span>
