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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422190"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="49c41-102">Obmedziť SharePoint Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="49c41-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="49c41-103">Niektoré organizácie stále vyžaduje klasický režim skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="49c41-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="49c41-104">Neexistujú žiadne plány na odstránenie klasického režimu granulovaného úrovni, od apríla 1,2019, to už nebude možné obmedziť celú organizáciu (nájomca) na klasický režim pre zoznamy a knižnice.</span><span class="sxs-lookup"><span data-stu-id="49c41-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="49c41-105">Admin bude mať nasledujúce možnosti spravovať jednotlivé zoznamy a knižnice v klasickom režime pomocou granulovaného odhlásiť prepínačov, ktoré poskytujeme na nasledujúcich úrovniach:</span><span class="sxs-lookup"><span data-stu-id="49c41-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="49c41-106">kolekcie lokalít</span><span class="sxs-lookup"><span data-stu-id="49c41-106">site collection</span></span>
- <span data-ttu-id="49c41-107">stránky</span><span class="sxs-lookup"><span data-stu-id="49c41-107">site</span></span>
- <span data-ttu-id="49c41-108">Zoznam</span><span class="sxs-lookup"><span data-stu-id="49c41-108">list</span></span>
- <span data-ttu-id="49c41-109">Knižnica</span><span class="sxs-lookup"><span data-stu-id="49c41-109">library</span></span>

<span data-ttu-id="49c41-110">Navyše, zoznamov, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modern sa stále automaticky prepne na klasický režim.</span><span class="sxs-lookup"><span data-stu-id="49c41-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="49c41-111">Po 1.apríla, zoznamov a knižníc, ktoré sú v klasickom režime v dôsledku neúčasti nájomca bude automaticky riadené na úrovni lokality a úroveň zoznamu.</span><span class="sxs-lookup"><span data-stu-id="49c41-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="49c41-112">Ak požadujete klasický režim nájdete viac informácií tu a PnP Powershell inštrukcie tu, ktorá opisuje možnosti a nástroje môžete použiť dnes pripraviť na odstránenie nájomcu úrovni opt-out 1 apríla.</span><span class="sxs-lookup"><span data-stu-id="49c41-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
