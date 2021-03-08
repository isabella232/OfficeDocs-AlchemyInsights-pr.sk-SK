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
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Správy odoslané skupine v Microsoft 365 nedostanú všetci členovia

Uistite sa, že všetci členovia skupiny majú zapnutý odber e-mailov. Pozrite si tému [Sledovanie skupiny v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Ak chcete skontrolovať stav správy členov, ktorí majú zapnutý odber e-mailov skupiny, spustite nasledujúci príkaz v prostredí [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Pomocou nasledujúceho príkazu prostredia PowerShell EXO nakonfigurujte všetkých členov skupiny na prijímanie e-mailov odoslaných skupine v Microsoft 365 do priečinka doručenej pošty:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Príklad:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`