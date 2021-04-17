---
title: Vyhľadávanie obsahu bez výsledkov
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816863"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="3b9c3-102">Žiadne výsledky vyhľadávania a exportov obsahu</span><span class="sxs-lookup"><span data-stu-id="3b9c3-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="3b9c3-103">Problémy s vyhľadávaním a exportmi obsahu, pri ktorých sa vracajú žiadne údaje, môže spôsobovať určitý filter zabezpečenia súladu, ktorý nastavuje konkrétny správca a ktorý ho nekomunikuje všetkým správcom.</span><span class="sxs-lookup"><span data-stu-id="3b9c3-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="3b9c3-104">Ak chcete vyriešiť tento problém, skontrolujte, či to môžu spôsobovať niektoré filtre zabezpečenia súladu:</span><span class="sxs-lookup"><span data-stu-id="3b9c3-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="3b9c3-105">Pripojenie k centre zabezpečenia a dodržiavania súladu v prostredí Powershell</span><span class="sxs-lookup"><span data-stu-id="3b9c3-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="3b9c3-106">Spustite nasledujúce commandlety:</span><span class="sxs-lookup"><span data-stu-id="3b9c3-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="3b9c3-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="3b9c3-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="3b9c3-108">Get-ComplianceSecurityFilter – Organizácia $org</span><span class="sxs-lookup"><span data-stu-id="3b9c3-108">Get-ComplianceSecurityFilter -Organization $org</span></span>