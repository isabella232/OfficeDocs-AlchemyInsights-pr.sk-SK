---
title: Obsah sa nezobrazuje vo výsledkoch vyhľadávania služby SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705676"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="97580-102">Obsah sa nezobrazuje vo výsledkoch vyhľadávania služby SharePoint</span><span class="sxs-lookup"><span data-stu-id="97580-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="97580-103">Postupujte podľa týchto krokov na riešenie problémov, keď očakávaný obsah nezobrazuje vo výsledkoch vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="97580-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="97580-104">Skontrolujte, či **lokalita** , ktorá obsahuje očakávaný obsah, je nastavená na umožnenie zobrazovania obsahu vo výsledkoch vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97580-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="97580-105">Postupujte podľa krokov v zozname [Zobraziť obsah na lokalite vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="97580-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="97580-106">Skontrolujte, či **zoznam** alebo **knižnica** , ktorá obsahuje očakávaný obsah, je nastavená na povolenie obsahu, ktorý sa má zobraziť vo výsledkoch vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97580-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="97580-107">Postupujte podľa krokov v zozname [Zobraziť obsah zo zoznamov alebo knižníc vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="97580-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="97580-108">Overte, či sa stránka, dokument alebo vlastné rozloženie strany publikujú ako **hlavná verzia.**</span><span class="sxs-lookup"><span data-stu-id="97580-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="97580-109">Postupujte krok 3 vo [vyhľadávaní nevráti všetky výsledky SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="97580-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="97580-110">Overte, či má používateľ **povolenia** na zobrazenie obsahu.</span><span class="sxs-lookup"><span data-stu-id="97580-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="97580-111">Postupujte podľa krokov v [porozumení úrovne povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="97580-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="97580-112">Ak schéma vyhľadávania bola zmenená pridaním novej spravovanej vlastnosti, úpravou spravovanej vlastnosti alebo odstránením spravovanej vlastnosti, požiada sa o prehľadávanie obsahu a opätovný index.</span><span class="sxs-lookup"><span data-stu-id="97580-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="97580-113">**Znova indexovať** obsah podľa krokov v [manuálnej požiadavke prehľadávania a opätovného indexovania lokality, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="97580-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="97580-114">Môže to chvíľu trvať, počkajte 24 hodín pred opätovným skontrolovaním výsledkov.</span><span class="sxs-lookup"><span data-stu-id="97580-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="97580-115">Ďalšie informácie nájdete v téme [povolenie vyhľadávania obsahu na lokalite](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="97580-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
