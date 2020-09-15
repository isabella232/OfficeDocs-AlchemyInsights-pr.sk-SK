---
title: Dynamics 365 – nesprávna tabuľa sa zobrazuje v systéme Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711290"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c7696-102">Nesprávna tabuľa sa zobrazuje v rozhraní Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="c7696-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c7696-103">Existuje niekoľko dôvodov, prečo sa môže zobraziť iná tabuľa, než očakávate:</span><span class="sxs-lookup"><span data-stu-id="c7696-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c7696-104">Používateľ nastavil predvolenú tabuľu používateľa</span><span class="sxs-lookup"><span data-stu-id="c7696-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c7696-105">Zvyčajne je možné identifikovať predvolenú tabuľu používateľa, ak sa na paneli príkazov tabule nezobrazuje tlačidlo **nastaviť ako predvolené** .</span><span class="sxs-lookup"><span data-stu-id="c7696-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c7696-106">Predvolenou tabuľou používateľa sa prepíšu všetky ostatné predvolené tabule, a to aj v prípade, že predvolená tabuľa používateľa sa nenachádza v aktuálnej aplikácii.</span><span class="sxs-lookup"><span data-stu-id="c7696-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c7696-107">Ak chcete zrušiť predvolenú tabuľu, použite toto alternatívne riešenie.</span><span class="sxs-lookup"><span data-stu-id="c7696-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c7696-108">Vytvorte novú osobnú tabuľu.</span><span class="sxs-lookup"><span data-stu-id="c7696-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c7696-109">Nastavte novú tabuľu ako predvolenú používateľa.</span><span class="sxs-lookup"><span data-stu-id="c7696-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c7696-110">Odstráňte túto tabuľu.</span><span class="sxs-lookup"><span data-stu-id="c7696-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c7696-111">Tabuľa sa nastavuje v súbore Sitemap</span><span class="sxs-lookup"><span data-stu-id="c7696-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c7696-112">Možno ste nastavili predvolenú tabuľu organizácie výberom tabule a výberom položky nastaviť ako predvolené v časti Prispôsobenie systému.</span><span class="sxs-lookup"><span data-stu-id="c7696-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c7696-113">Tabuľa definovaná v návrhárovi Sitemap však bude mať prednosť pred touto tabuľou, ak má k nemu prístup používateľ.</span><span class="sxs-lookup"><span data-stu-id="c7696-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c7696-114">Ak chcete, aby sa používateľom zobrazila tabuľa, ktorú ste nastavili ako predvolenú organizáciu, môžete buď:</span><span class="sxs-lookup"><span data-stu-id="c7696-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c7696-115">Nastavenie tejto tabule v Sitemap</span><span class="sxs-lookup"><span data-stu-id="c7696-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c7696-116">Odstránenie prístupu k súboru Sitemap definovaného tabuľa pre týchto používateľov</span><span class="sxs-lookup"><span data-stu-id="c7696-116">Remove access to the sitemap defined dashboard for those users</span></span>
