---
title: Obnovenie odstránených položiek pomocou rutiny cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493430"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="b454b-102">Obnovenie odstránených položiek pomocou rutiny cmdlet</span><span class="sxs-lookup"><span data-stu-id="b454b-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="b454b-103">Pomocou rutiny cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) zobrazte odstránené položky v poštových schránkach.</span><span class="sxs-lookup"><span data-stu-id="b454b-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="b454b-104">Po vyhľadaní odstránených položiek, môžete ich [obnoviť-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) rutiny cmdlet obnoviť.</span><span class="sxs-lookup"><span data-stu-id="b454b-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="b454b-105">Pozrite si všetky podrobnosti v [get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b454b-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="b454b-106">Pred spustením tejto rutiny cmdlet je potrebné priradiť rolu Export importu poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="b454b-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="b454b-107">Ďalšie informácie nájdete v téme [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="b454b-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
