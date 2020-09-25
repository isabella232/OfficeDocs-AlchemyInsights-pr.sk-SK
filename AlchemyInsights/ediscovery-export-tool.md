---
title: nástroj na exportovanie eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277934"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="53d3e-102">Nedá sa nainštalovať alebo spustiť nástroj na exportovanie elektronického vyhľadávania?</span><span class="sxs-lookup"><span data-stu-id="53d3e-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="53d3e-103">Ak nemôžete nainštalovať alebo spustiť nástroj na exportovanie eDiscovery na stiahnutie výsledkov vyhľadávania, pozrite si nasledujúce skutočnosti:</span><span class="sxs-lookup"><span data-stu-id="53d3e-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="53d3e-104">Počítač, ktorý používate, spĺňa tieto požiadavky:</span><span class="sxs-lookup"><span data-stu-id="53d3e-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="53d3e-105">32 alebo 64-bitové verzie Windowsu 7 a novších verzií</span><span class="sxs-lookup"><span data-stu-id="53d3e-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="53d3e-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="53d3e-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="53d3e-107">Podporovaný prehliadač:</span><span class="sxs-lookup"><span data-stu-id="53d3e-107">A supported browser:</span></span>

  - <span data-ttu-id="53d3e-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="53d3e-108">Microsoft Edge</span></span>

    <span data-ttu-id="53d3e-109">Alebo</span><span class="sxs-lookup"><span data-stu-id="53d3e-109">Or</span></span>

  - <span data-ttu-id="53d3e-110">Internet Explorer 10 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="53d3e-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="53d3e-111">Ďalšie prehliadače, ako je napríklad Google Chrome a Mozilla Firefox, nie sú podporované.</span><span class="sxs-lookup"><span data-stu-id="53d3e-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="53d3e-112">Vaša organizácia sa môže pripojiť ku koncovému bodu v Azure, ktorý je \*\* \* . blob.Core.Windows.net\*\* (zástupný znak predstavuje jedinečný identifikátor pre úlohu exportu).</span><span class="sxs-lookup"><span data-stu-id="53d3e-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="53d3e-113">Ste priradili rolu exportu v &amp; Centre zabezpečenia dodržiavania súladu pre Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="53d3e-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="53d3e-114">Predvolene je táto rola priradená k skupine rolí správcu eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="53d3e-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="53d3e-115">Pozrite si tému [Priradenie povolení pre eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="53d3e-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="53d3e-116">Ďalšie informácie nájdete v téme [exportovanie výsledkov vyhľadávania obsahu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="53d3e-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="53d3e-117">Ak exportujete viac než 100K poštových schránok, budete musieť použiť nasledujúce prostredie PowerShell na stiahnutie výsledkov exportu:  [exportovanie výsledkov z viac ako 100k poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="53d3e-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>