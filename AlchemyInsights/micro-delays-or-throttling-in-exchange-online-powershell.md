---
title: Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702141"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="4ba7a-102">Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4ba7a-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="4ba7a-103">Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="4ba7a-104">Tu je niekoľko návrhov, ako to vyriešiť:</span><span class="sxs-lookup"><span data-stu-id="4ba7a-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="4ba7a-105">Spustením našich diagnostiky uvoľnite politiky obmedzovania prostredia PowerShell nájomníka.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="4ba7a-106">Toto riešenie najviac vyrieši problém.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="4ba7a-107">Ak sa problém nevyriešil, použite [modul Exchange Online v2 Prostredia PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ktorý obsahuje cmDlety, ktoré sú založené na rozhraní REST API a sú výrazne výkonnejšie.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="4ba7a-108">Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="4ba7a-109">Ak potrebujete použiť príkazy CMDlets, ktoré nie sú zahrnuté v module V2, pozrite si časť Spustenie rutín typu cmdlet prostredia PowerShell pre veľký počet používateľov v prostredí [Office 365,](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ktorá hovorí o tom, ako obísť limity obmedzovania prostredia PowerShell v prostredí Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4ba7a-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
