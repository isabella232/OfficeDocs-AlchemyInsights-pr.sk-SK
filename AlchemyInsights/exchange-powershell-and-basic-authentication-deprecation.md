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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="9b626-102">Exchange PowerShell a ukončenie základného overovania</span><span class="sxs-lookup"><span data-stu-id="9b626-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="9b626-103">Najnovšie informácie o tom, ako sa pripojiť do prostredia Exchange Online PowerShell bez použitia základného overovania, [nájdete tu](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="9b626-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="9b626-104">Nezabúdajte, že v klientskom počítači musí byť stále povolené základné overenie.</span><span class="sxs-lookup"><span data-stu-id="9b626-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="9b626-105">Nový modul PowerShell v2 využíva Modern Auth na vytvorenie pripojenia, ktoré umožní všetky rutiny typu V2 Cmdlets typu REST.</span><span class="sxs-lookup"><span data-stu-id="9b626-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="9b626-106">Okrem rutín typu V2 cmdlets vám umožňuje aj prístup k rutinám typu Remote PowerShell (RPS) Cmdletsm ktoré vyžadujú, aby bola spustená relácia Remote PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="9b626-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="9b626-107">Na vytvorenie relácie RPS na zariadení Windows sa vyžaduje, aby bola povolená možnosť WinRM BasicAuth na klientskom zariadení, aj keď modul na overenie služby používa mechanizmus Modern Auth.</span><span class="sxs-lookup"><span data-stu-id="9b626-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="9b626-108">Kanál WinRM Basic Auth sa používa na prenos tokenov Modern Auth.</span><span class="sxs-lookup"><span data-stu-id="9b626-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="9b626-109">Ak je WinRM Basic Auth v klientskom zariadení vypnuté, nové rutiny typu V2 cmdlet budú fungovať aj naďalej (staršie rutín typu RPS cmdlet však nebudú).</span><span class="sxs-lookup"><span data-stu-id="9b626-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
