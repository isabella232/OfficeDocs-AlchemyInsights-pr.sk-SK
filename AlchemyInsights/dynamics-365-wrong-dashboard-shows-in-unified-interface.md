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
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748689"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="d2ba0-102">Zle dashboard zobrazuje v Dynamics 365 jednotné rozhranie</span><span class="sxs-lookup"><span data-stu-id="d2ba0-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="d2ba0-103">Existuje niekoľko dôvodov, prečo môžete vidieť odlišné dashboard než očakávate:</span><span class="sxs-lookup"><span data-stu-id="d2ba0-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="d2ba0-104">Používateľ má nastaviť predvolenú používateľskú tabuľu</span><span class="sxs-lookup"><span data-stu-id="d2ba0-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="d2ba0-105">Zvyčajne môžete identifikovať užívateľa predvolenú tabuľu je nastavená, ak tlačidlo **Nastaviť ako predvolené** neukazuje v dashboard panel príkazov.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="d2ba0-106">Predvolenú používateľskú tabuľu prepíšu všetky ostatné predvolené tabule, aj keď používateľ predvolenú tabuľu nie je v aktuálnej aplikácii.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="d2ba0-107">Použiť nasledovné riešenie na odstavenie ich predvolenú tabuľu.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="d2ba0-108">Vytvoriť nový osobný dashboard.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="d2ba0-109">Nastaviť že nový dashboard ako používateľom predvolený program.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="d2ba0-110">Odstránenie tejto tabule.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="d2ba0-111">Panel je nastavený v sitemap</span><span class="sxs-lookup"><span data-stu-id="d2ba0-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="d2ba0-112">Možno ste nastavili organizácie predvolenú tabuľu výberom tabule a položky "Nastaviť ako predvolené" pod "Prispôsobenie systému".</span><span class="sxs-lookup"><span data-stu-id="d2ba0-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="d2ba0-113">Ale tabuľa definovaná v návrhárovi sitemap budú mať prednosť pred túto tabuľu, ak používateľ má prístup k nemu.</span><span class="sxs-lookup"><span data-stu-id="d2ba0-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="d2ba0-114">Aby užívatelia panel ste nastavili ako predvolené nastavenie organizácie, môžete buď:</span><span class="sxs-lookup"><span data-stu-id="d2ba0-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="d2ba0-115">Nastaví túto tabuľu v sitemap</span><span class="sxs-lookup"><span data-stu-id="d2ba0-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="d2ba0-116">Odstrániť prístup na sitemap definované tabuľu pre tých užívateľov</span><span class="sxs-lookup"><span data-stu-id="d2ba0-116">Remove access to the sitemap defined dashboard for those users</span></span>
