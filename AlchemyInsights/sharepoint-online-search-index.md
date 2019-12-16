---
title: Vyhľadávanie v SharePointe Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044058"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="1ee6f-102">Prehľadávanie obsahu a indexovanie v SharePointe Online</span><span class="sxs-lookup"><span data-stu-id="1ee6f-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="1ee6f-103">Obsah musí byť prehľadávaný a pridaný do vyhľadávacieho indexu pre používateľov nájsť to, čo hľadajú v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="1ee6f-104">Obsah sa automaticky prehľadávajú na základe vopred definovaného plánu prehľadávania obsahu (plán prehľadávania obsahu sa nedá zmeniť).</span><span class="sxs-lookup"><span data-stu-id="1ee6f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="1ee6f-105">Prehľadávač sníma obsah, ktorý sa zmenil od posledného prehľadávania obsahu a aktualizuje index.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="1ee6f-106">Na zabezpečenie obsahu prehľadané a index je aktualizovaný, Všimnite si nasledujúce:</span><span class="sxs-lookup"><span data-stu-id="1ee6f-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="1ee6f-107">Uistite sa, že obsah možno nájsť tým, že [obsah stránky vyhľadávať](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="1ee6f-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="1ee6f-108">Keď ste zmenili spravovanú vlastnosť, alebo keď ste zmenili mapovanie prehľadávaných a spravovaných vlastností, lokalita musí byť znovu prehľadávané predtým, ako sa zmeny prejavia vo vyhľadávacom indexe.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="1ee6f-109">Pretože zmeny sú vykonané v schéme vyhľadávania, a nie na skutočnú lokalitu, prehľadávač nebude automaticky znova indexovať lokality.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="1ee6f-110">Ďalšie informácie nájdete v téme [manuálne vyžiadanie prehľadávania a opätovného indexovania lokality, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="1ee6f-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="1ee6f-111">Počkajte aspoň 24 hodín po manuálnom vyžiadaní prehľadávania obsahu a úplného opätovného indexu, aby ste zistili, či sa stále vyskytol problém.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="1ee6f-112">Ak uplynulo viac ako 24 hodín od začatia prehľadávania obsahu a úplného opätovného indexovania, prihláste sa na podporu prípadu.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="1ee6f-113">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1ee6f-114">Prosím, dajte nám aspoň 24 hodín na dokončenie riešenia.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1ee6f-115">Ak lokalita, dokument (Knižnica) alebo zoznam bol odstránený a stále zobrazuje vo výsledkoch vyhľadávania, používatelia by sa mali zobraziť **chyba 404 súbor sa nenašiel** pri pokuse o prístup.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="1ee6f-116">Tento problém by mal byť prihlásený ako podporný prípad pre ďalšie vyšetrovanie.</span><span class="sxs-lookup"><span data-stu-id="1ee6f-116">This issue should be logged as a support case for further investigation.</span></span> 



