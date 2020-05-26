---
title: Uvítacia správa v Microsoft 365 skupiny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358339"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="587a8-102">Uvítacia správa v Microsoft 365 skupiny</span><span class="sxs-lookup"><span data-stu-id="587a8-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="587a8-103">Noví používatelia, ktorí sa pripojili k skupine Microsoft 365, dostanú uvítací e-mail, ak je vlastnosť "UnifiedGroupWelcomeMessageEnabled" pravdivá.</span><span class="sxs-lookup"><span data-stu-id="587a8-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="587a8-104">V prípade, že chcete vypnúť uvítaciu správu, použite nasledovný príkaz [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) :</span><span class="sxs-lookup"><span data-stu-id="587a8-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
