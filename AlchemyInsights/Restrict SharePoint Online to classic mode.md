---
title: Obmedziť SharePoint Online na klasický režim
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953359"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="e44d3-102">Obmedziť SharePoint Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="e44d3-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="e44d3-103">Niektoré organizácie stále vyžaduje klasický režim skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="e44d3-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="e44d3-104">Neexistujú žiadne plány na odstránenie klasického režimu granulovaného úrovni, od apríla 1,2019, to už nebude možné obmedziť celú organizáciu (nájomca) na klasický režim pre zoznamy a knižnice.</span><span class="sxs-lookup"><span data-stu-id="e44d3-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="e44d3-105">Admin bude mať nasledujúce možnosti spravovať jednotlivé zoznamy a knižnice v klasickom režime pomocou granulovaného odhlásiť prepínačov, ktoré poskytujeme na nasledujúcich úrovniach:</span><span class="sxs-lookup"><span data-stu-id="e44d3-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="e44d3-106">--zoznam lokalít zberu--stránky----Knižnica</span><span class="sxs-lookup"><span data-stu-id="e44d3-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="e44d3-107">Navyše, zoznamov, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modern sa stále automaticky prepne na klasický režim.</span><span class="sxs-lookup"><span data-stu-id="e44d3-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="e44d3-108">Po 1.apríla, zoznamov a knižníc, ktoré sú v klasickom režime v dôsledku neúčasti nájomca bude automaticky riadené na úrovni lokality a úroveň zoznamu.</span><span class="sxs-lookup"><span data-stu-id="e44d3-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="e44d3-109">Ak požadujete klasický režim nájdete viac informácií tu a PnP Powershell inštrukcie tu, ktorá opisuje možnosti a nástroje môžete použiť dnes pripraviť na odstránenie nájomcu úrovni opt-out 1 apríla.</span><span class="sxs-lookup"><span data-stu-id="e44d3-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
