---
title: Exchange PowerShell a ukončenie základného overovania
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
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015704"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell a ukončenie základného overovania

Najnovšie informácie o tom, ako sa pripojiť do prostredia Exchange Online PowerShell bez použitia základného overovania, [nájdete tu](https://aka.ms/psbasicauth).

Nezabúdajte, že v klientskom počítači musí byť stále povolené základné overenie.
Nový modul PowerShell v2 využíva Modern Auth na vytvorenie pripojenia, ktoré umožní všetky rutiny typu V2 Cmdlets typu REST. Okrem rutín typu V2 cmdlets vám umožňuje aj prístup k rutinám typu Remote PowerShell (RPS) Cmdletsm ktoré vyžadujú, aby bola spustená relácia Remote PowerShellu. Na vytvorenie relácie RPS na zariadení Windows sa vyžaduje, aby bola povolená možnosť WinRM BasicAuth na klientskom zariadení, aj keď modul na overenie služby používa mechanizmus Modern Auth. Kanál WinRM Basic Auth sa používa na prenos tokenov Modern Auth. Ak je WinRM Basic Auth v klientskom zariadení vypnuté, nové rutiny typu V2 cmdlet budú fungovať aj naďalej (staršie rutín typu RPS cmdlet však nebudú).
