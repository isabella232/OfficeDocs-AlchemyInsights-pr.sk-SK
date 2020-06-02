---
title: 1491-vyhľadávanie-ne-návrat-očakávané výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510587"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="9e6c9-102">Vyhľadávanie obsahu nevracia očakávané výsledky</span><span class="sxs-lookup"><span data-stu-id="9e6c9-102">Content Search not returning expected results</span></span>

<span data-ttu-id="9e6c9-103">Pri spustení vyhľadávania obsahu z Microsoft 365 zabezpečenia & Compliance Center, môže sa zobraziť neočakávané výsledky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="9e6c9-104">Zvážte nasledujúce možnosti, ktoré môžu ovplyvniť výsledky vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="9e6c9-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="9e6c9-105">**Umiestnenia obsahu a podmienky vyhľadávania**: Uistite sa, že ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="9e6c9-106">Ak ste spustili veľké vyhľadávanie (s mnohými umiestneniami), zvážte jeho rozdelenie na viacero vyhľadávaní.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="9e6c9-107">**Čiastočne indexované položky**: [Čiastočne indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté vo výsledkoch odhadovaného vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="9e6c9-108">Čiastočne indexované položky z lokalít SharePointu a OneDrivu však nie sú zahrnuté do odhadu vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="9e6c9-109">**Zlyhania vyhľadávania**: Pri vyhľadávaní veľkého počtu poštových schránok (viac ako 100 000 poštových schránok) sa môžu zobraziť chyby vyhľadávania s chybovými kódmi, ako sú CS008-009 a CS012-002).</span><span class="sxs-lookup"><span data-stu-id="9e6c9-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="9e6c9-110">V takom prípade zopakujte vyhľadávanie len pre neúspešné umiestnenia obsahu.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="9e6c9-111">Ďalšie informácie nájdete v [tomto článku.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)</span><span class="sxs-lookup"><span data-stu-id="9e6c9-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
