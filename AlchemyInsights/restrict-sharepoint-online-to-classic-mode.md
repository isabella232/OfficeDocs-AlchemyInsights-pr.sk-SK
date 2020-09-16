---
title: Obmedziť SharePoint Online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751437"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="4b2ef-102">Obmedziť SharePoint Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="4b2ef-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="4b2ef-103">Niektoré organizácie vyžadujú klasické používanie režimu.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="4b2ef-104">Hoci neexistujú žiadne plány na odstránenie klasického režimu na úrovni zrnitosti, už nie je možné obmedziť celú organizáciu (nájomníka) na klasický režim pre zoznamy a knižnice.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="4b2ef-105">Správca bude mať k dispozícii nasledujúce možnosti na spravovanie jednotlivých zoznamov a knižníc v klasickom režime pomocou granulovaných prepínačov opt-out, ktoré poskytujeme na nasledujúcich úrovniach:</span><span class="sxs-lookup"><span data-stu-id="4b2ef-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="4b2ef-106">kolekcia lokalít</span><span class="sxs-lookup"><span data-stu-id="4b2ef-106">site collection</span></span>
- <span data-ttu-id="4b2ef-107">stránky</span><span class="sxs-lookup"><span data-stu-id="4b2ef-107">site</span></span>
- <span data-ttu-id="4b2ef-108">zoznamu</span><span class="sxs-lookup"><span data-stu-id="4b2ef-108">list</span></span>
- <span data-ttu-id="4b2ef-109">Knižnica</span><span class="sxs-lookup"><span data-stu-id="4b2ef-109">library</span></span>

<span data-ttu-id="4b2ef-110">Okrem toho zoznamy, ktoré používajú určité funkcie a prispôsobenia, ktoré nie sú podporované modernými, budú automaticky prepnutý do klasického režimu.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="4b2ef-111">Začiatok apríla 1, 2019, proces vypnutia úrovne nájomníka opt out of Modern zoznam a knižnice sa spustí a pokračuje až do 31. mája 2019.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="4b2ef-112">Zoznamy a knižnice, ktoré sa nachádzajú v klasickom režime ako výsledok opt-out nájomníka, sa automaticky presunú do modernej.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="4b2ef-113">Ak potrebujete klasický režim, prečítajte [si tu ďalšie informácie a](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) [v tomto článku](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) nájdete informácie o možnostiach a nástrojoch, ktoré môžete použiť na používanie klasického režimu.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
