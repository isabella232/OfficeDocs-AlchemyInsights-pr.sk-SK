---
title: Vyhľadávanie v službe SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059267"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="7fafc-102">Vyhľadávanie v službe SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7fafc-102">Search in SharePoint Online</span></span>

<span data-ttu-id="7fafc-103">Obsah musí prechádzať a pridali do vyhľadávacieho indexu užívateľom nájsť, čo hľadajú v SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7fafc-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="7fafc-104">Automaticky prehľadávania obsahu založené na vopred definovaných crawl plán (plán prehľadávania obsahu nie je možné zmeniť).</span><span class="sxs-lookup"><span data-stu-id="7fafc-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="7fafc-105">Modul na prehľadávanie obsahu sa zdvihne obsah, ktorý sa zmenil od posledného prehľadávania a aktualizuje register.</span><span class="sxs-lookup"><span data-stu-id="7fafc-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="7fafc-106">Na zabezpečenie prehľadávania obsahu a aktualizácia registra prebieha, uvedomte si nasledovné:</span><span class="sxs-lookup"><span data-stu-id="7fafc-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="7fafc-107">Uistite sa, že obsah možno nájsť tým, [že obsah stránky vyhľadávať](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="7fafc-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="7fafc-108">Keď ste zmenili spravovanú vlastnosť, alebo keď ste zmenili mapovanie liezol a spravované vlastnosti, stránky musí byť opätovne prehľadaný pred zmeny sa prenesú do indexu vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="7fafc-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="7fafc-109">Pretože vaše zmeny v schéme Hľadať, a nie skutočné stránky, crawler nebude automaticky znovu index stránky.</span><span class="sxs-lookup"><span data-stu-id="7fafc-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="7fafc-110">Ďalšie informácie nájdete v téme [manuálne požiadať o plazenie a opätovné indexovanie stránky, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="7fafc-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="7fafc-111">Počkajte aspoň 24 hodín po manuálne požiadať plaziť a plné re-index vidieť, ak máte stále problém.</span><span class="sxs-lookup"><span data-stu-id="7fafc-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="7fafc-112">Ak od uskutočnenia prehľadávania obsahu a plnej preindexovania spracoval uplynulo viac ako 24 hodín, prihláste sa podpory prípadu.</span><span class="sxs-lookup"><span data-stu-id="7fafc-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="7fafc-113">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="7fafc-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7fafc-114">Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.</span><span class="sxs-lookup"><span data-stu-id="7fafc-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Dôležité!]<span data-ttu-id="7fafc-115">: Ak stránky, dokumentu (Knižnica) alebo zoznam bol odstránený a stále ukazuje vo výsledkoch vyhľadávania, používatelia by mali dostávať **Chyba 404 súbor nebol nájdený** pri pokuse o prístup.</span><span class="sxs-lookup"><span data-stu-id="7fafc-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="7fafc-116">Tento problém sa zapíšu ako prípad pre ďalšie vyšetrovanie.</span><span class="sxs-lookup"><span data-stu-id="7fafc-116">This issue should be logged as a support case for further investigation.</span></span> 



