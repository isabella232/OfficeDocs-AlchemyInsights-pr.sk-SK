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
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761774"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="0f1bb-102">Obmedziť SharePoint Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="0f1bb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="0f1bb-103">Niektoré organizácie stále vyžaduje klasický režim skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="0f1bb-104">Neexistujú žiadne plány na odstránenie klasického režimu granulovaného úrovni, už nie je možné obmedziť celú organizáciu (nájomca) na klasický režim pre zoznamy a knižnice.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="0f1bb-105">Admin bude mať nasledujúce možnosti spravovať jednotlivé zoznamy a knižnice v klasickom režime pomocou granulovaného odhlásiť prepínačov, ktoré poskytujeme na nasledujúcich úrovniach:</span><span class="sxs-lookup"><span data-stu-id="0f1bb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="0f1bb-106">kolekcie lokalít</span><span class="sxs-lookup"><span data-stu-id="0f1bb-106">site collection</span></span>
- <span data-ttu-id="0f1bb-107">stránky</span><span class="sxs-lookup"><span data-stu-id="0f1bb-107">site</span></span>
- <span data-ttu-id="0f1bb-108">Zoznam</span><span class="sxs-lookup"><span data-stu-id="0f1bb-108">list</span></span>
- <span data-ttu-id="0f1bb-109">Knižnica</span><span class="sxs-lookup"><span data-stu-id="0f1bb-109">library</span></span>

<span data-ttu-id="0f1bb-110">Navyše, zoznamov, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modern sa stále automaticky prepne na klasický režim.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="0f1bb-111">Začiatok 1 Máj 2019, proces vypnúť nájomcu úrovni odhlásiť moderné zoznamu a knižnice začať a pokračovať cez 31 mája 2019.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="0f1bb-112">Zoznamy a knižnice, ktoré sú v klasickom režime v dôsledku neúčasti nájomca bude automaticky presunul do modernej.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="0f1bb-113">Ak požadujete klasický režim nájdete viac informácií [tu](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) a PnP Powershell inštrukcie [tu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) popisujúci možnosti a nástroje, ktoré môžete použiť dnes využiť skúsenosti klasický režim.</span><span class="sxs-lookup"><span data-stu-id="0f1bb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
