---
title: Správy odoslané skupine v Microsoft 365 nedostanú všetci členovia
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976520"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Správy odoslané skupine v Microsoft 365 nedostanú všetci členovia

Uistite sa, že všetci členovia skupiny majú zapnutý odber e-mailov. Pozrite si tému [Sledovanie skupiny v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Ak chcete skontrolovať stav správy členov, ktorí majú zapnutý odber e-mailov skupiny, spustite nasledujúci príkaz v prostredí [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Pomocou nasledujúceho príkazu prostredia PowerShell EXO nakonfigurujte všetkých členov skupiny na prijímanie e-mailov odoslaných skupine v Microsoft 365 do priečinka doručenej pošty:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Príklad:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`