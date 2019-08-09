---
title: Spravovať schéma vyhľadávania SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270145"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="654ef-102">Spravovať schéma vyhľadávania SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="654ef-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="654ef-103">Schéma vyhľadávania ovláda používatelia môžu vyhľadávať, ako používatelia môžete vyhľadávať a ako budete prezentovať výsledky vyhľadávania webových lokalít.</span><span class="sxs-lookup"><span data-stu-id="654ef-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="654ef-104">Pozri [Spravovať schéma vyhľadávania SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) sa dozviete ako:</span><span class="sxs-lookup"><span data-stu-id="654ef-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="654ef-105">Zmene schéma vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="654ef-105">Change the search schema.</span></span>
- <span data-ttu-id="654ef-106">Vytváranie spravovaných vlastností.</span><span class="sxs-lookup"><span data-stu-id="654ef-106">Create managed properties.</span></span>
- <span data-ttu-id="654ef-107">Mapa prehľadávané prehľadávané vlastnosti k spravovaným vlastnostiam.</span><span class="sxs-lookup"><span data-stu-id="654ef-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="654ef-108">Uvedomte si nasledujúcu k ťažkostiam riadenia schéma vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="654ef-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="654ef-109">Ak dostanete upozornenie, **Aplikácia je pozastavené** pri zmena schémy, to je len dočasné ako je služba údržby dochádza.</span><span class="sxs-lookup"><span data-stu-id="654ef-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="654ef-110">Ak uplynulo viac ako 24 hodín a stále narazíte na upozornenie, prihláste sa podpory prípadu.</span><span class="sxs-lookup"><span data-stu-id="654ef-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="654ef-111">Keď zmeníte spravované vlastnosti alebo pridať nové, zmeny sa prejavia až po obsah bol opätovne prehľadaný.</span><span class="sxs-lookup"><span data-stu-id="654ef-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="654ef-112">SharePoint Online, plazenie sa deje automaticky podľa na pláne definovaných crawl.</span><span class="sxs-lookup"><span data-stu-id="654ef-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="654ef-113">Uistite sa, že zmeny sú liezol, môžete konkrétne [žiadosti opätovné indexovanie zoznamu alebo knižnice](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="654ef-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="654ef-114">Kompletný prehľad schéma vyhľadávania, nájdete [Predstavujeme schéma vyhľadávania](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="654ef-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


