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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell

Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia. Tu je niekoľko návrhov, ako to vyriešiť:

- Spustením našich diagnostiky uvoľnite politiky obmedzovania prostredia PowerShell nájomníka. Toto riešenie najviac vyrieši problém.
- Ak sa problém nevyriešil, použite [modul Exchange Online v2 Prostredia PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ktorý obsahuje cmDlety, ktoré sú založené na rozhraní REST API a sú výrazne výkonnejšie. Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.
- Ak potrebujete použiť príkazy CMDlets, ktoré nie sú zahrnuté v module V2, pozrite si časť Spustenie rutín typu cmdlet prostredia PowerShell pre veľký počet používateľov v prostredí [Office 365,](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ktorá hovorí o tom, ako obísť limity obmedzovania prostredia PowerShell v prostredí Exchange Online.
