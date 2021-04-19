---
title: Exchange PowerShell a ukončenie základného overovania
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
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813487"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell a ukončenie základného overovania

Najnovšie informácie o tom, ako sa pripojiť do prostredia Exchange Online PowerShell bez použitia základného overovania, [nájdete tu](https://aka.ms/exops-docs). Modul PowerShell V2 nepodporuje základné overovanie.

Nezabúdajte, že v klientskom počítači musí byť stále povolené základné overenie.
Nový modul PowerShell v2 využíva Modern Auth na vytvorenie pripojenia, ktoré umožní všetky rutiny typu V2 Cmdlets typu REST. Okrem rutín typu V2 cmdlets vám umožňuje aj prístup k rutinám typu Remote PowerShell (RPS) Cmdletsm ktoré vyžadujú, aby bola spustená relácia Remote PowerShellu. Na vytvorenie relácie RPS na zariadení Windows sa vyžaduje, aby bola povolená možnosť WinRM BasicAuth na klientskom zariadení, aj keď modul na overenie služby používa mechanizmus Modern Auth. Kanál WinRM Basic Auth sa používa na prenos tokenov Modern Auth. Ak je WinRM Basic Auth v klientskom zariadení vypnuté, nové rutiny typu V2 cmdlet budú fungovať aj naďalej (staršie rutín typu RPS cmdlet však nebudú).
