---
title: 1491-Search-not-Returning-Expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776096"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="ea29f-102">Obsah vyhľadávanie nevracajú očakávané výsledky</span><span class="sxs-lookup"><span data-stu-id="ea29f-102">Content Search not returning expected results</span></span>

<span data-ttu-id="ea29f-103">Pri spustení obsah vyhľadávanie od & Office 365 zabezpečenia súladu Center, dostanete neočakávané výsledky.</span><span class="sxs-lookup"><span data-stu-id="ea29f-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="ea29f-104">Zoberme si nasledujúce veci, ktoré môžu ovplyvniť výsledky vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="ea29f-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="ea29f-105">**Umiestnenia obsahu a podmienok vyhľadávania**: Uistite sa, že ste si vybrali správneho umiestnenia obsahu a vyhľadávanie podmienky.</span><span class="sxs-lookup"><span data-stu-id="ea29f-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="ea29f-106">Ak ste spustili veľké vyhľadávanie (s mnohých miestach), zvážte ju rozdeliť na niekoľko prehliadok.</span><span class="sxs-lookup"><span data-stu-id="ea29f-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="ea29f-107">**Čiastočne indexované položky**: [čiastočne indexované položky](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) zo schránky sú zahrnuté vo výsledkoch vyhľadávania odhadované.</span><span class="sxs-lookup"><span data-stu-id="ea29f-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="ea29f-108">Však čiastočne indexované položky z lokalít v službe SharePoint a OneDrive nie sú zahrnuté v odhade Hľadať.</span><span class="sxs-lookup"><span data-stu-id="ea29f-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="ea29f-109">**Vyhľadávanie porúch**: pri hľadaní veľkého počtu poštových schránok (viac ako 100.000 schránky), dostanete Hľadať chyby, kódy chýb ako je CS008-009 a CS012-002).</span><span class="sxs-lookup"><span data-stu-id="ea29f-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="ea29f-110">V takom prípade zopakujte hľadanie zlyhalo obsah umiestnenia.</span><span class="sxs-lookup"><span data-stu-id="ea29f-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="ea29f-111">Pozri [Tento článok](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="ea29f-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
