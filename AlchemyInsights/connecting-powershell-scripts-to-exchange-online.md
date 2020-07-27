---
title: Pripojenie skriptov prostredia PowerShell k službe Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 34301e62a25e11c5d4c353166f8208ef74245dfa
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423779"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="1c4ee-102">Pripojenie skriptov prostredia PowerShell k službe Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1c4ee-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="1c4ee-103">Základné overovanie v službe Exchange Online bude zastarané a cesta vpred je pripojiť pomocou overovania na základe certifikátu pre skripty a bezobslužné úlohy.</span><span class="sxs-lookup"><span data-stu-id="1c4ee-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="1c4ee-104">Ďalšie informácie nájdete v [téme Overovanie iba pre aplikácie pre bezobslužné skripty v module EXO V2](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span><span class="sxs-lookup"><span data-stu-id="1c4ee-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>