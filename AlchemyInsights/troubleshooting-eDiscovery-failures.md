---
title: 1490 – riešenie problémov – eDiscovery – zlyhanie
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277840"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="0fc97-102">Riešenie chýb vyhľadávania obsahu</span><span class="sxs-lookup"><span data-stu-id="0fc97-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="0fc97-103">Vyskytli sa problémy pri vyhľadávaní obsahu alebo pri exportovaní výsledkov vyhľadávania?</span><span class="sxs-lookup"><span data-stu-id="0fc97-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="0fc97-104">Zobrazuje sa vám napríklad nasledovné pri spustení vyhľadávania?</span><span class="sxs-lookup"><span data-stu-id="0fc97-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="0fc97-105">CS008 alebo CS012 chyby</span><span class="sxs-lookup"><span data-stu-id="0fc97-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="0fc97-106">Chyby na serveri zaneprázdnený/timeout</span><span class="sxs-lookup"><span data-stu-id="0fc97-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="0fc97-107">Vyskytla sa chyba aplikácie</span><span class="sxs-lookup"><span data-stu-id="0fc97-107">Application error occurred</span></span>

<span data-ttu-id="0fc97-108">Alebo pri vyhľadávaní alebo exportovaní výsledkov z veľkého počtu poštových schránok (cez 100 000 poštových schránok) sa zobrazujú chyby exportu?</span><span class="sxs-lookup"><span data-stu-id="0fc97-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="0fc97-109">Pri týchto typoch chýb skúste zopakovať hľadanie umiestnení obsahu, ktoré zlyhali.</span><span class="sxs-lookup"><span data-stu-id="0fc97-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="0fc97-110">Ďalšie informácie nájdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="0fc97-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="0fc97-111">Ak exportujete viac než 100K poštových schránok, budete musieť použiť nasledujúce prostredie PowerShell na stiahnutie výsledkov exportu:  [exportovanie výsledkov z viac ako 100k poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0fc97-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
