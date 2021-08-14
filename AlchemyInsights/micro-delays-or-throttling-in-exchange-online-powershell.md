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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868549"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro oneskorenia alebo obmedzovanie v prostredí Exchange Online PowerShell

Pri spustení skriptov a rutín typu cmdlet v službe Exchange Online sa môžu vyskytnúť upozornenia „Micro Delay Applied“ (Použilo sa mikro oneskorenie) alebo oneskorenia. Tu je niekoľko návrhov, ako to vyriešiť:

- Spustením našich diagnostiky uvoľnite politiky obmedzovania prostredia PowerShell nájomníka. Toto riešenie najviac vyrieši problém.
- Ak sa problém nevyriešil, použite [modul Exchange Online v2 prostredia PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ktorý obsahuje cmDlety, ktoré sú založené na rozhraní REST API a sú výrazne výkonnejšie. Môže to byť skvelé riešenie v prípade mnohých rutín typu Get- CMDlet, ktoré sa používajú často.
- Ak potrebujete použiť cmDlets, ktoré nie sú zahrnuté v module V2, pozrite si časť Spustenie rutín typu cmdlet prostredia PowerShell pre veľký počet používateľov v prostredí [Office 365,](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ktorá hovorí o tom, ako obísť limity obmedzovania prostredia PowerShell v prostredí Exchange Online.
