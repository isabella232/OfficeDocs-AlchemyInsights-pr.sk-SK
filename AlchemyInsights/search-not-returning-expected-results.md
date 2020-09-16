---
title: 1491 – vyhľadávanie – nevracajú sa – očakávané – výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740489"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a4384-102">Vyhľadávanie obsahu nevracia očakávané výsledky</span><span class="sxs-lookup"><span data-stu-id="a4384-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a4384-103">Pri spúšťaní vyhľadávania obsahu z centra zabezpečenia & zabezpečenia spoločnosti Microsoft 365 sa môžu zobraziť neočakávané výsledky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="a4384-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a4384-104">Zvážte nasledujúce skutočnosti, ktoré môžu ovplyvniť výsledky vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="a4384-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a4384-105">**Umiestnenia obsahu a podmienky vyhľadávania**: Skontrolujte, či ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="a4384-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a4384-106">Ak ste spustili veľké vyhľadávanie (s mnohými umiestneniami), zvážte rozdelenie na viacero vyhľadávaní.</span><span class="sxs-lookup"><span data-stu-id="a4384-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a4384-107">**Čiastočne indexované položky**:  [čiastočne indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté v odhadovaných výsledkoch hľadania.</span><span class="sxs-lookup"><span data-stu-id="a4384-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a4384-108">Čiastočne indexované položky z lokalít v SharePointe a OneDrive však nie sú zahrnuté v odhade vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="a4384-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a4384-109">**Zlyhanie vyhľadávania**: pri vyhľadávaní veľkého počtu poštových schránok (cez 100 000 poštových schránok) sa môžu zobraziť chyby vyhľadávania s kódmi chýb, ako sú napríklad CS008-009 a CS012-002).</span><span class="sxs-lookup"><span data-stu-id="a4384-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a4384-110">V tomto prípade zopakujte vyhľadávanie len v prípade zlyhaných umiestnení obsahu.</span><span class="sxs-lookup"><span data-stu-id="a4384-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a4384-111">Ďalšie informácie nájdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="a4384-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
