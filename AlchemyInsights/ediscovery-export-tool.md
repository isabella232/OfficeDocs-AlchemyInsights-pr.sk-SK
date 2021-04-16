---
title: Nástroj na exportovanie eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814603"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="7c041-102">Nemôžete nainštalovať alebo spustiť nástroj na exportovanie eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="7c041-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="7c041-103">Ak nemôžete nainštalovať alebo spustiť nástroj na exportovanie eDiscovery a stiahnuť výsledky vyhľadávania, skontrolujte tieto veci:</span><span class="sxs-lookup"><span data-stu-id="7c041-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="7c041-104">Počítač, ktorý používate, spĺňa tieto požiadavky:</span><span class="sxs-lookup"><span data-stu-id="7c041-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="7c041-105">32-bitová alebo 64-bitová verzia Windowsu 7 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="7c041-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="7c041-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="7c041-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="7c041-107">Podporovaný prehliadač:</span><span class="sxs-lookup"><span data-stu-id="7c041-107">A supported browser:</span></span>

  - <span data-ttu-id="7c041-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="7c041-108">Microsoft Edge</span></span>

    <span data-ttu-id="7c041-109">Alebo</span><span class="sxs-lookup"><span data-stu-id="7c041-109">Or</span></span>

  - <span data-ttu-id="7c041-110">Internet Explorer 10 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="7c041-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="7c041-111">Iné prehliadače, napríklad Google Chrome a Mozilla Firefox, nie sú podporované.</span><span class="sxs-lookup"><span data-stu-id="7c041-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="7c041-112">Vaša organizácia sa môže pripojiť ku koncovmu bodu v službe Azure, čo je **\* .blob.core.windows.net** (zástupný znak predstavuje jedinečný identifikátor úlohy exportu).</span><span class="sxs-lookup"><span data-stu-id="7c041-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="7c041-113">V Centre zabezpečenia služieb Microsoft 365 máte priradenú rolu &amp; exportu.</span><span class="sxs-lookup"><span data-stu-id="7c041-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="7c041-114">Táto rola je predvolene priradená len skupine rolí eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="7c041-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="7c041-115">Pozrite si [časť Priradenie povolení na eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="7c041-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="7c041-116">Ďalšie informácie nájdete v téme [Export výsledkov vyhľadávania obsahu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="7c041-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="7c041-117">Ak exportujete viac ako 100 000 poštových schránok, na stiahnutie výsledkov exportu budete musieť použiť toto prostredie PowerShell: Export výsledkov z viac ako  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)poštových schránok.</span><span class="sxs-lookup"><span data-stu-id="7c041-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>