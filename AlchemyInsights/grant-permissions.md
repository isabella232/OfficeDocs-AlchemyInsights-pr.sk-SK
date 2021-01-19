---
title: Udelenie povolení
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901615"
---
# <a name="grant-permissions"></a><span data-ttu-id="75e2e-102">Udelenie povolení</span><span class="sxs-lookup"><span data-stu-id="75e2e-102">Grant permissions</span></span>

1. <span data-ttu-id="75e2e-103">**Udelenie súhlasu správcu na úrovni nájomníka**: [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) informácie o udelení súhlasu správcu v rámci celého nájomníka nájdete v téme podrobné pokyny na udelenie súhlasu správcu v celom nájomníkovi na portáli Azure pomocou prostredia Azure AD PowerShell alebo z výzvy na súhlas.</span><span class="sxs-lookup"><span data-stu-id="75e2e-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="75e2e-104">**Udelenie súhlasu v mene konkrétneho používateľa**: namiesto udelenia súhlasu pre celú organizáciu môže správca tiež použiť [rozhranie Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) na udelenie súhlasu s delegovanými povoleniami v mene jedného používateľa.</span><span class="sxs-lookup"><span data-stu-id="75e2e-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="75e2e-105">Ďalšie informácie nájdete v téme [získanie prístupu v mene používateľa](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="75e2e-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>