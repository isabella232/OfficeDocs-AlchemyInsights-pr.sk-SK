---
title: 1491-Search-not-vracajúci sa-očakávané-výsledky
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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709242"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="97341-102">Vyhľadávanie obsahu nevracia očakávané výsledky</span><span class="sxs-lookup"><span data-stu-id="97341-102">Content Search not returning expected results</span></span>

<span data-ttu-id="97341-103">Pri spustení vyhľadávania obsahu z Microsoft 365 zabezpečenia & Compliance Center, môže sa zobraziť neočakávané výsledky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97341-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="97341-104">Zvážte nasledujúce veci, ktoré môžu ovplyvniť výsledky vyhľadávania:</span><span class="sxs-lookup"><span data-stu-id="97341-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="97341-105">**Umiestnenia obsahu a podmienky vyhľadávania**: Skontrolujte, či ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97341-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="97341-106">Ak ste spustili veľké vyhľadávanie (s mnohými miestami), zvážte rozdelenie do viacerých vyhľadávaní.</span><span class="sxs-lookup"><span data-stu-id="97341-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="97341-107">**Čiastočne indexované položky**: [čiastočne indexované položky](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté v odhadovaných výsledkoch vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97341-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="97341-108">Čiastočne indexované položky z lokalít SharePoint a OneDrive však nie sú zahrnuté do odhadu vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97341-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="97341-109">**Zlyhanie vyhľadávania**: pri hľadaní veľkého počtu poštových schránok (viac ako 100 000 poštových schránok) sa môžu získať chyby vyhľadávania s kódmi chýb, ako sú napríklad CS008-009 a CS012-002).</span><span class="sxs-lookup"><span data-stu-id="97341-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="97341-110">V tomto prípade zopakujte vyhľadávanie len pre neúspešné umiestnenia obsahu.</span><span class="sxs-lookup"><span data-stu-id="97341-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="97341-111">Pozri [Tento článok](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="97341-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
