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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964959"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="139d4-102">Obsah vyhľadávanie nevracajú očakávané výsledky</span><span class="sxs-lookup"><span data-stu-id="139d4-102">Content Search not returning expected results</span></span>

<span data-ttu-id="139d4-p101">Pri spustení obsah vyhľadávanie od & Office 365 zabezpečenia súladu Center, dostanete neočakávané výsledky. Zoberme si nasledujúce veci, ktoré môžu ovplyvniť výsledky vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="139d4-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="139d4-p102">**Umiestnenia obsahu a podmienok vyhľadávania**: Uistite sa, že ste si vybrali správneho umiestnenia obsahu a vyhľadávanie podmienky. Ak ste spustili veľké vyhľadávanie (s mnohých miestach), zvážte ju rozdeliť na niekoľko prehliadok.</span><span class="sxs-lookup"><span data-stu-id="139d4-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="139d4-p103">**Čiastočne indexované položky**: [čiastočne indexované položky](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) zo schránky sú zahrnuté vo výsledkoch vyhľadávania odhadované. Však čiastočne indexované položky z lokalít v službe SharePoint a OneDrive nie sú zahrnuté v odhade Hľadať.</span><span class="sxs-lookup"><span data-stu-id="139d4-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="139d4-p104">**Vyhľadávanie porúch**: pri hľadaní veľkého počtu poštových schránok (viac ako 100.000 schránky), dostanete Hľadať chyby, kódy chýb ako je CS008-009 a CS012-002). V takom prípade zopakujte hľadanie zlyhalo obsah umiestnenia. Pozri [Tento článok](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="139d4-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
