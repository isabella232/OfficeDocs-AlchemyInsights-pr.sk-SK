---
title: Správa slovníkov vyhľadávania SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758780"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="873ef-102">Vyhľadávanie v službe SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="873ef-102">Search in SharePoint Online</span></span>

<span data-ttu-id="873ef-103">Obsah musí prechádzať a pridali do vyhľadávacieho indexu užívateľom nájsť, čo hľadajú v SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="873ef-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="873ef-104">Automaticky prehľadávania obsahu založené na vopred definovaných crawl plán (plán prehľadávania obsahu nie je možné zmeniť).</span><span class="sxs-lookup"><span data-stu-id="873ef-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="873ef-105">Modul na prehľadávanie obsahu sa zdvihne obsah, ktorý sa zmenil od posledného prehľadávania a aktualizuje register.</span><span class="sxs-lookup"><span data-stu-id="873ef-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="873ef-106">Na zabezpečenie prehľadávania obsahu a aktualizuje index, postupujte podľa nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="873ef-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="873ef-107">Uistite sa, že obsah možno nájsť tým, že obsah stránky vyhľadávať.</span><span class="sxs-lookup"><span data-stu-id="873ef-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="873ef-108">Ďalšie informácie nájdete v téme [povolenie obsah stránky byť prehľadávateľné](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="873ef-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="873ef-109">Keď ste zmenili spravovanú vlastnosť, alebo keď ste zmenili mapovanie liezol a spravované vlastnosti, stránky musí byť opätovne prehľadaný pred zmeny sa prenesú do indexu vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="873ef-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="873ef-110">Pretože vaše zmeny v schéme Hľadať, a nie skutočné stránky, crawler nebude automaticky znovu index stránky.</span><span class="sxs-lookup"><span data-stu-id="873ef-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="873ef-111">Ďalšie informácie nájdete v téme [manuálne požiadať o plazenie a opätovné indexovanie stránky, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="873ef-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="873ef-112">Počkajte aspoň 24 hodín po manuálne požiadať plaziť a plné re-index vidieť, ak máte stále problém.</span><span class="sxs-lookup"><span data-stu-id="873ef-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="873ef-113">Ak od uskutočnenia prehľadávania obsahu a plnej preindexovania spracoval uplynulo viac ako 24 hodín, prihláste sa podpory prípadu.</span><span class="sxs-lookup"><span data-stu-id="873ef-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="873ef-114">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="873ef-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="873ef-115">Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.</span><span class="sxs-lookup"><span data-stu-id="873ef-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="873ef-116">**Dôležité**: Ak stránky, dokumentu (Knižnica) alebo zoznam bol odstránený a stále ukazuje vo výsledkoch vyhľadávania, používatelia by mali dostať chyba 404 súbor nebol nájdený pri pokuse o prístup.</span><span class="sxs-lookup"><span data-stu-id="873ef-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="873ef-117">Tento problém sa zapíšu ako prípad pre ďalšie vyšetrovanie.</span><span class="sxs-lookup"><span data-stu-id="873ef-117">This issue should be logged as a support case for further investigation.</span></span> 



