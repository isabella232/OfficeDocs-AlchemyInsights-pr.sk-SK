---
title: Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750016"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="6370e-102">Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii</span><span class="sxs-lookup"><span data-stu-id="6370e-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="6370e-103">Vykonajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="6370e-103">Follow these steps:</span></span>

1. <span data-ttu-id="6370e-104">Ak nie ste globálnym správcom, môžete vyhľadávať správy, ktoré je potrebné pridať do **skupiny rolí správcu eDiscovery** alebo na **rolu správy vyhľadávania súladu**.</span><span class="sxs-lookup"><span data-stu-id="6370e-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="6370e-105">Ak chcete odstrániť správy, budete sa musieť zapojiť do **skupiny rolí Správa organizácie** alebo do **roly riadenia vyhľadávania a čistenia**.</span><span class="sxs-lookup"><span data-stu-id="6370e-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="6370e-106">Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia & compliance.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="6370e-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="6370e-107">Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/office365/securitycompliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="6370e-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="6370e-108">[Pripojte sa k zabezpečeniu & prostredie centrum dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6370e-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="6370e-109">Ak používate MFA, prečítajte si tieto pokyny: [pripojenie k zabezpečeniu & centrum dodržiavania súladu v prostredí s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="6370e-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="6370e-110">Odstránenie správy: `New-ComplianceSearchAction` Ak chcete správu odstrániť, spustite rutinu typu cmdlet.</span><span class="sxs-lookup"><span data-stu-id="6370e-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="6370e-111">Odstránené správy sa presunú do priečinka s využiteľnými položkami používateľa.</span><span class="sxs-lookup"><span data-stu-id="6370e-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="6370e-112">Príkaz príklad nájdete v časti [Krok 3: odstránenie správy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="6370e-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
