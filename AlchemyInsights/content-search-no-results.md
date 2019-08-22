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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516794"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="dcc4d-102">Žiadne výsledky z obsahu vyhľadávanie/vývoz</span><span class="sxs-lookup"><span data-stu-id="dcc4d-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="dcc4d-103">Problémy s obsahom Hľadať/vývoz nevracajú žiadne údaje môžu byť spôsobené určité súlad Filter zabezpečenia, ktorý bol konkrétne Admin a nekomunikuje pre všetky adminy.</span><span class="sxs-lookup"><span data-stu-id="dcc4d-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="dcc4d-104">Ak chcete vyriešiť tento problém, skontrolujte, ak existuje súlad bezpečnostné filtre, ktoré môžu byť príčinou:</span><span class="sxs-lookup"><span data-stu-id="dcc4d-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="dcc4d-105">Pripojiť k bezpečnosti a centrum súladu Powershell</span><span class="sxs-lookup"><span data-stu-id="dcc4d-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="dcc4d-106">Spustite nasledujúce riešenia:</span><span class="sxs-lookup"><span data-stu-id="dcc4d-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="dcc4d-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="dcc4d-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="dcc4d-108">Get-ComplianceSecurityFilter-organizácia $org</span><span class="sxs-lookup"><span data-stu-id="dcc4d-108">Get-ComplianceSecurityFilter -Organization $org</span></span>