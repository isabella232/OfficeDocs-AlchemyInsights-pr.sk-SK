---
title: Vyhľadávanie obsahu žiadne výsledky
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680662"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="acf6f-102">Žiadne výsledky z vyhľadávania obsahu alebo exportu</span><span class="sxs-lookup"><span data-stu-id="acf6f-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="acf6f-103">Problémy s vyhľadávaním obsahu alebo exportovaním, ktoré nevracajú žiadne údaje, môžu byť spôsobené niektorými filtrami zabezpečenia súladu, ktorý bol nastavením konkrétneho správcu, a nekomunikoval ho so všetkými správcami.</span><span class="sxs-lookup"><span data-stu-id="acf6f-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="acf6f-104">Ak chcete tento problém vyriešiť, skontrolujte, či sa nenachádzajú žiadne filtre zabezpečenia dodržiavania súladu, ktoré môžu spôsobovať toto:</span><span class="sxs-lookup"><span data-stu-id="acf6f-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="acf6f-105">Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="acf6f-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="acf6f-106">Spustite nasledovné príkazové aplety:</span><span class="sxs-lookup"><span data-stu-id="acf6f-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="acf6f-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="acf6f-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="acf6f-108">Get-ComplianceSecurityFilter-organizácia $org</span><span class="sxs-lookup"><span data-stu-id="acf6f-108">Get-ComplianceSecurityFilter -Organization $org</span></span>