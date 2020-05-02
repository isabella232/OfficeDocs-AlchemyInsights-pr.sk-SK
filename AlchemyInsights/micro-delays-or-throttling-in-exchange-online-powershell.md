---
title: Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948032"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="b81ad-102">Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="b81ad-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="b81ad-103">Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia.</span><span class="sxs-lookup"><span data-stu-id="b81ad-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="b81ad-104">V súvislosti s týmto ponúkame dva návrhy:</span><span class="sxs-lookup"><span data-stu-id="b81ad-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="b81ad-105">Možno budete chcieť skúsiť použitie [modulu Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), ktorý obsahuje rutiny typu CMDlet založené na rozhraní REST API, ktoré sú oveľa výkonnejšie.</span><span class="sxs-lookup"><span data-stu-id="b81ad-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="b81ad-106">Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.</span><span class="sxs-lookup"><span data-stu-id="b81ad-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="b81ad-107">Ak potrebujete používať rutiny typu CMDlet, ktoré zatiaľ nie sú zahrnuté v module v2, pozrite si tému [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) (Spustenie rutín typu cmdlet prostredia PowerShell pre veľké množstvo používateľov v Office 365), v ktorej sa dozviete, ako obísť očakávané limity a obmedzenia prostredia PowerShell v službe Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b81ad-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
