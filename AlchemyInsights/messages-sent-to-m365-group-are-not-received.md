---
title: Správy odoslané do skupiny Microsoft 365 nie sú prijaté všetci členovia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: sk-SK
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051516"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="c218e-102">Správy odoslané do skupiny Microsoft 365 nie sú prijaté všetci členovia</span><span class="sxs-lookup"><span data-stu-id="c218e-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="c218e-103">Uistite sa, že všetci členovia skupiny sa prihlásili na odber e-mailov.</span><span class="sxs-lookup"><span data-stu-id="c218e-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="c218e-104">Ďalšie informácie sa nachádzajú [v téme Sledovanie skupiny v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="c218e-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="c218e-105">Ak chcete skontrolovať stav správy členov, ktorí sa prihlásili na odber skupinových e-mailov, spustite nasledujúci príkaz na [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="c218e-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`