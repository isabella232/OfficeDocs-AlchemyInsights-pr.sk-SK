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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell

Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia. V súvislosti s týmto ponúkame dva návrhy:

- Možno budete chcieť skúsiť použitie [modulu Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), ktorý obsahuje rutiny typu CMDlet založené na rozhraní REST API, ktoré sú oveľa výkonnejšie. Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.
- Ak potrebujete používať rutiny typu CMDlet, ktoré zatiaľ nie sú zahrnuté v module v2, pozrite si tému [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) (Spustenie rutín typu cmdlet prostredia PowerShell pre veľké množstvo používateľov v Office 365), v ktorej sa dozviete, ako obísť očakávané limity a obmedzenia prostredia PowerShell v službe Exchange Online.
