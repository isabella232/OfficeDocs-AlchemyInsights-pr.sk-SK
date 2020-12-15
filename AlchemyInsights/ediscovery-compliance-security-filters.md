---
title: Pri vyhľadávaní obsahu alebo exportovaní sa nevrátia žiadne výsledky
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680327"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="cd2f2-102">Pri vyhľadávaní obsahu alebo exportovaní sa nevrátia žiadne výsledky</span><span class="sxs-lookup"><span data-stu-id="cd2f2-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="cd2f2-103">Ak sa vyskytnú problémy s nasledujúcimi scenármi eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="cd2f2-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="cd2f2-104">Vyhľadávanie obsahu/export vráti žiadne údaje ani neočakávané údaje</span><span class="sxs-lookup"><span data-stu-id="cd2f2-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="cd2f2-105">Vyhľadávanie eDiscovery alebo export zlyhá</span><span class="sxs-lookup"><span data-stu-id="cd2f2-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="cd2f2-106">Môže to byť spôsobené určitými filtrami zabezpečenia súladu, ktoré boli nastavené konkrétnym správcom, a neboli oznámené všetkým správcom.</span><span class="sxs-lookup"><span data-stu-id="cd2f2-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="cd2f2-107">Ak chcete tento problém vyriešiť, skontrolujte, či sú k dispozícii žiadne filtre zabezpečenia súladu, ktoré môžu spôsobovať tieto problémy:</span><span class="sxs-lookup"><span data-stu-id="cd2f2-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="cd2f2-108">Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="cd2f2-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="cd2f2-109">Spustite nasledovné príkazové aplety:</span><span class="sxs-lookup"><span data-stu-id="cd2f2-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="cd2f2-110">Ďalšie informácie o filtroch zabezpečenia dodržiavania súladu nájdete v téme [filtrovanie povolení na vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="cd2f2-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
