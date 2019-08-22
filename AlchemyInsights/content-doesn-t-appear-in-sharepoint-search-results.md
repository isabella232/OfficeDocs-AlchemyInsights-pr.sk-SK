---
title: Obsah sa nezobrazí vo výsledkoch vyhľadávania SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517046"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="7647b-102">Obsah sa nezobrazí vo výsledkoch vyhľadávania SharePoint</span><span class="sxs-lookup"><span data-stu-id="7647b-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="7647b-103">Postupujte podľa týchto krokov, ak sa nezobrazuje očakávaný obsah vo výsledkoch vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="7647b-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="7647b-104">Skontrolujte, či **stránka** , ktorá obsahuje očakávaný obsah je nastavený na Povoliť obsah zobrazovať vo výsledkoch vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="7647b-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7647b-105">Postupujte podľa [Zobraziť obsah na mieste vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7647b-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="7647b-106">Skontrolujte, že **zoznam** alebo **knižnicu** , ktorá obsahuje očakávaný obsah je nastavený na Povoliť obsah zobrazovať vo výsledkoch vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="7647b-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7647b-107">Postupujte podľa [Zobraziť obsah zo zoznamov alebo knižníc vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7647b-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="7647b-108">Overiť, že stránky, dokumentu alebo vlastné rozloženie je publikovaná ako **hlavná verzia.**</span><span class="sxs-lookup"><span data-stu-id="7647b-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="7647b-109">Postupujte podľa kroku 3 v [hľadanie nevrátilo všetky výsledky SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="7647b-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="7647b-110">Overte, či má používateľ **povolenia** na zobrazenie obsahu.</span><span class="sxs-lookup"><span data-stu-id="7647b-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="7647b-111">Postupujte podľa [chápanie úrovní povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="7647b-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="7647b-112">Ak schéma vyhľadávania bol zmenený pridaním novú spravovanú vlastnosť, upravovať spravovanú vlastnosť alebo odstránením spravovanú vlastnosť potom žiada plaziť a preindexuje bude vyžadovať.</span><span class="sxs-lookup"><span data-stu-id="7647b-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="7647b-113">**Opätovné indexovanie** obsahu podľa krokov uvedených v téme [manuálne požiadať o plazenie a opätovné indexovanie stránky, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="7647b-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="7647b-114">To môže chvíľu trvať, počkajte 24 hodín pred zisťovaním výsledkov znova.</span><span class="sxs-lookup"><span data-stu-id="7647b-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="7647b-115">Ďalšie informácie nájdete v téme [povolenie obsah stránky byť prehľadávateľné](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="7647b-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
