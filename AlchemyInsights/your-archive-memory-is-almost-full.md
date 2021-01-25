---
title: Archívna poštová schránka je takmer plná
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974663"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="eb029-102">Archívna poštová schránka je takmer plná</span><span class="sxs-lookup"><span data-stu-id="eb029-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="eb029-103">Ak používateľ dostane upozornenie, **Archívna poštová schránka je takmer plná** alebo potrebujete zväčšiť veľkosť svojej archívnej poštovej schránky, tu je niekoľko tipov:</span><span class="sxs-lookup"><span data-stu-id="eb029-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="eb029-104">Ak má používateľ priradenú Exchange Online (plán 1), inovujte na licenciu na **Exchange Online Plan 2** a zvýšte veľkosť zo 50 GB na 100 GB.</span><span class="sxs-lookup"><span data-stu-id="eb029-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="eb029-105">Ak je už používateľ priradený k niektorej z týchto možností: **Exchange Online Plan 2** alebo Exchange Online (plán 1) pomocou doplnku Exchange Online archivácia, pomocou nasledujúcich krokov môžete povoliť automatické rozšírenie archivácie:.</span><span class="sxs-lookup"><span data-stu-id="eb029-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="eb029-106">[Pripojte sa k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="eb029-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="eb029-107">Spustite nasledovné Group pre používateľa:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="eb029-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="eb029-108">Ak chcete potvrdiť, že je pre používateľa povolená, spustite nasledujúce Group:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="eb029-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="eb029-109">Ďalšie informácie nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="eb029-109">For more information see:</span></span>

- [<span data-ttu-id="eb029-110"> Povolenie neobmedzenej archivácie – Pomocník pre správcov – Microsoft 365 Compliance | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="eb029-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="eb029-111">Limity služby Exchange Online – popisy služieb | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="eb029-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="eb029-112">Inovácia na iný podnikový plán | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="eb029-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

