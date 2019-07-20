---
title: Žiadne výsledky vyhľadávania obsahu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800586"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="873d9-102">Žiadne výsledky z obsahu vyhľadávanie/vývoz</span><span class="sxs-lookup"><span data-stu-id="873d9-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="873d9-103">Problémy s obsahom Hľadať/vývoz nevracajú žiadne údaje môžu byť spôsobené určité súlad Filter zabezpečenia, ktorý bol konkrétne Admin a nekomunikuje pre všetky adminy.</span><span class="sxs-lookup"><span data-stu-id="873d9-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="873d9-104">Ak chcete vyriešiť tento problém, skontrolujte, ak existuje súlad bezpečnostné filtre, ktoré môžu byť príčinou:</span><span class="sxs-lookup"><span data-stu-id="873d9-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="873d9-105">Pripojiť k bezpečnosti a centrum súladu Powershell</span><span class="sxs-lookup"><span data-stu-id="873d9-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="873d9-106">Spustite nasledujúce riešenia:</span><span class="sxs-lookup"><span data-stu-id="873d9-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="873d9-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="873d9-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="873d9-108">Get-ComplianceSecurityFilter-organizácia $org</span><span class="sxs-lookup"><span data-stu-id="873d9-108">Get-ComplianceSecurityFilter -Organization $org</span></span>