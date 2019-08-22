---
title: Dynamics 365 - zle Dashboard zobrazuje v Dynamics 365 jednotné rozhranie
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528566"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="5d910-102">Zle dashboard zobrazuje v Dynamics 365 jednotné rozhranie</span><span class="sxs-lookup"><span data-stu-id="5d910-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="5d910-103">Existuje niekoľko dôvodov, prečo môžete vidieť odlišné dashboard než očakávate:</span><span class="sxs-lookup"><span data-stu-id="5d910-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="5d910-104">Používateľ má nastaviť predvolenú používateľskú tabuľu</span><span class="sxs-lookup"><span data-stu-id="5d910-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="5d910-105">Zvyčajne môžete identifikovať užívateľa predvolenú tabuľu je nastavená, ak tlačidlo **Nastaviť ako predvolené** neukazuje v dashboard panel príkazov.</span><span class="sxs-lookup"><span data-stu-id="5d910-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="5d910-106">Predvolenú používateľskú tabuľu prepíšu všetky ostatné predvolené tabule, aj keď používateľ predvolenú tabuľu nie je v aktuálnej aplikácii.</span><span class="sxs-lookup"><span data-stu-id="5d910-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="5d910-107">Použiť nasledovné riešenie na odstavenie ich predvolenú tabuľu.</span><span class="sxs-lookup"><span data-stu-id="5d910-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="5d910-108">Vytvoriť nový osobný dashboard.</span><span class="sxs-lookup"><span data-stu-id="5d910-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="5d910-109">Nastaviť že nový dashboard ako používateľom predvolený program.</span><span class="sxs-lookup"><span data-stu-id="5d910-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="5d910-110">Odstránenie tejto tabule.</span><span class="sxs-lookup"><span data-stu-id="5d910-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="5d910-111">Panel je nastavený v sitemap</span><span class="sxs-lookup"><span data-stu-id="5d910-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="5d910-112">Možno ste nastavili organizácie predvolenú tabuľu výberom tabule a položky "Nastaviť ako predvolené" pod "Prispôsobenie systému".</span><span class="sxs-lookup"><span data-stu-id="5d910-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="5d910-113">Ale tabuľa definovaná v návrhárovi sitemap budú mať prednosť pred túto tabuľu, ak používateľ má prístup k nemu.</span><span class="sxs-lookup"><span data-stu-id="5d910-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="5d910-114">Aby užívatelia panel ste nastavili ako predvolené nastavenie organizácie, môžete buď:</span><span class="sxs-lookup"><span data-stu-id="5d910-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="5d910-115">Nastaví túto tabuľu v sitemap</span><span class="sxs-lookup"><span data-stu-id="5d910-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="5d910-116">Odstrániť prístup na sitemap definované tabuľu pre tých užívateľov</span><span class="sxs-lookup"><span data-stu-id="5d910-116">Remove access to the sitemap defined dashboard for those users</span></span>
