---
title: Správy odoslané skupine v Microsoft 365 nedostanú všetci členovia
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480698"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="e2318-102">Správy odoslané skupine v Microsoft 365 nedostanú všetci členovia</span><span class="sxs-lookup"><span data-stu-id="e2318-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="e2318-103">Uistite sa, že všetci členovia skupiny majú zapnutý odber e-mailov.</span><span class="sxs-lookup"><span data-stu-id="e2318-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="e2318-104">Pozrite si tému [Sledovanie skupiny v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="e2318-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="e2318-105">Ak chcete skontrolovať stav správy členov, ktorí majú zapnutý odber e-mailov skupiny, spustite nasledujúci príkaz v prostredí [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="e2318-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="e2318-106">Pomocou nasledujúceho príkazu prostredia PowerShell EXO nakonfigurujte všetkých členov skupiny na prijímanie e-mailov odoslaných skupine v Microsoft 365 do priečinka doručenej pošty:</span><span class="sxs-lookup"><span data-stu-id="e2318-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="e2318-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="e2318-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`