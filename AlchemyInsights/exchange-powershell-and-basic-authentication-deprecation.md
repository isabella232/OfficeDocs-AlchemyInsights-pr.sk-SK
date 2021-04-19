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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="b82af-102">Exchange PowerShell a ukončenie základného overovania</span><span class="sxs-lookup"><span data-stu-id="b82af-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="b82af-103">Najnovšie informácie o tom, ako sa pripojiť do prostredia Exchange Online PowerShell bez použitia základného overovania, [nájdete tu](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="b82af-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="b82af-104">Modul PowerShell V2 nepodporuje základné overovanie.</span><span class="sxs-lookup"><span data-stu-id="b82af-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="b82af-105">Nezabúdajte, že v klientskom počítači musí byť stále povolené základné overenie.</span><span class="sxs-lookup"><span data-stu-id="b82af-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="b82af-106">Nový modul PowerShell v2 využíva Modern Auth na vytvorenie pripojenia, ktoré umožní všetky rutiny typu V2 Cmdlets typu REST.</span><span class="sxs-lookup"><span data-stu-id="b82af-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="b82af-107">Okrem rutín typu V2 cmdlets vám umožňuje aj prístup k rutinám typu Remote PowerShell (RPS) Cmdletsm ktoré vyžadujú, aby bola spustená relácia Remote PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="b82af-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="b82af-108">Na vytvorenie relácie RPS na zariadení Windows sa vyžaduje, aby bola povolená možnosť WinRM BasicAuth na klientskom zariadení, aj keď modul na overenie služby používa mechanizmus Modern Auth.</span><span class="sxs-lookup"><span data-stu-id="b82af-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="b82af-109">Kanál WinRM Basic Auth sa používa na prenos tokenov Modern Auth.</span><span class="sxs-lookup"><span data-stu-id="b82af-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="b82af-110">Ak je WinRM Basic Auth v klientskom zariadení vypnuté, nové rutiny typu V2 cmdlet budú fungovať aj naďalej (staršie rutín typu RPS cmdlet však nebudú).</span><span class="sxs-lookup"><span data-stu-id="b82af-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
