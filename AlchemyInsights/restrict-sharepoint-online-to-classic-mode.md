---
title: Obmedzenie lokality SharePoint Online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048775"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="70fc5-102">Obmedzenie lokality SharePoint Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="70fc5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="70fc5-103">Niektoré organizácie stále vyžadujú klasický režim skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="70fc5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="70fc5-104">Zatiaľ čo neexistujú žiadne plány na odstránenie klasického režimu na granulovanej úrovni, už nie je možné obmedziť celú organizáciu (nájomcu) na klasický režim pre zoznamy a knižnice.</span><span class="sxs-lookup"><span data-stu-id="70fc5-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="70fc5-105">Admin bude mať nasledujúce možnosti spravovať jednotlivé zoznamy a knižnice v klasickom režime pomocou podrobných opt-out prepínače, ktoré poskytujeme na týchto úrovniach:</span><span class="sxs-lookup"><span data-stu-id="70fc5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="70fc5-106">kolekcie lokalít</span><span class="sxs-lookup"><span data-stu-id="70fc5-106">site collection</span></span>
- <span data-ttu-id="70fc5-107">Stránky</span><span class="sxs-lookup"><span data-stu-id="70fc5-107">site</span></span>
- <span data-ttu-id="70fc5-108">Zoznam</span><span class="sxs-lookup"><span data-stu-id="70fc5-108">list</span></span>
- <span data-ttu-id="70fc5-109">Knižnica</span><span class="sxs-lookup"><span data-stu-id="70fc5-109">library</span></span>

<span data-ttu-id="70fc5-110">Okrem toho zoznamy, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modernými bude stále automaticky prepne do klasického režimu.</span><span class="sxs-lookup"><span data-stu-id="70fc5-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="70fc5-111">Začiatok apríla 1, 2019, proces vypnúť nájomcu úroveň opt out moderného zoznamu a knižníc začne a pokračovať až 31 mája 2019.</span><span class="sxs-lookup"><span data-stu-id="70fc5-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="70fc5-112">Zoznamy a knižnice, ktoré sú v klasickom režime v dôsledku odhlásenia nájomníka sa automaticky posunú na moderné.</span><span class="sxs-lookup"><span data-stu-id="70fc5-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="70fc5-113">Ak požadujete klasický režim, prečítajte si viac informácií [tu](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) a PNP PowerShell inštrukcie [tu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , ktorá opisuje možnosti a nástroje, ktoré môžete použiť dnes používať klasický režim skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="70fc5-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
