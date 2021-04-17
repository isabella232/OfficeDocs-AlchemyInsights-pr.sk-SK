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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830048"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell

Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia. V súvislosti s týmto ponúkame dva návrhy:

- Možno budete chcieť skúsiť použitie [modulu Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), ktorý obsahuje rutiny typu CMDlet založené na rozhraní REST API, ktoré sú oveľa výkonnejšie. Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.
- Ak potrebujete používať rutiny typu CMDlet, ktoré zatiaľ nie sú zahrnuté v module v2, pozrite si tému [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) (Spustenie rutín typu cmdlet prostredia PowerShell pre veľké množstvo používateľov v Office 365), v ktorej sa dozviete, ako obísť očakávané limity a obmedzenia prostredia PowerShell v službe Exchange Online.
