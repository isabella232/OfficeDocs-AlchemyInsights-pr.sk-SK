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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314715"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell

Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia. Tu je niekoľko návrhov, ako to vyriešiť:

- Spustením našich diagnostiky uvoľnite politiky obmedzovania prostredia PowerShell nájomníka. Toto riešenie najviac vyrieši problém.
- Ak sa problém nevyriešil, použite [modul Exchange Online v2 prostredia PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ktorý obsahuje cmDlety, ktoré sú založené na rozhraní REST API a sú výrazne výkonnejšie. Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.
- Ak potrebujete používať príkazy CMDlets, ktoré nie sú zahrnuté v module V2, pozrite si časť Spustenie rutín typu cmdlet prostredia PowerShell pre veľký počet používateľov v prostredí [Office 365,](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ktorá hovorí o tom, ako obísť limity obmedzovania prostredia PowerShell v Exchange Online.
