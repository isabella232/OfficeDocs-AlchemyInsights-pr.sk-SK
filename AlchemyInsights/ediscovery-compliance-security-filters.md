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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727238"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="6bf15-102">Pri vyhľadávaní obsahu alebo exportovaní sa nevrátia žiadne výsledky</span><span class="sxs-lookup"><span data-stu-id="6bf15-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="6bf15-103">Ak sa vyskytnú problémy s nasledujúcimi scenármi eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="6bf15-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="6bf15-104">Vyhľadávanie obsahu/export vráti žiadne údaje ani neočakávané údaje</span><span class="sxs-lookup"><span data-stu-id="6bf15-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="6bf15-105">Vyhľadávanie eDiscovery alebo export zlyhá</span><span class="sxs-lookup"><span data-stu-id="6bf15-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="6bf15-106">Môže to byť spôsobené určitými filtrami zabezpečenia súladu, ktoré boli nastavené konkrétnym správcom, a neboli oznámené všetkým správcom.</span><span class="sxs-lookup"><span data-stu-id="6bf15-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="6bf15-107">Ak chcete tento problém vyriešiť, skontrolujte, či sú k dispozícii žiadne filtre zabezpečenia súladu, ktoré môžu spôsobovať tieto problémy:</span><span class="sxs-lookup"><span data-stu-id="6bf15-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="6bf15-108">Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="6bf15-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="6bf15-109">Spustite nasledovné príkazové aplety:</span><span class="sxs-lookup"><span data-stu-id="6bf15-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="6bf15-110">Ďalšie informácie o filtroch zabezpečenia dodržiavania súladu nájdete v téme [filtrovanie povolení na vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="6bf15-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
