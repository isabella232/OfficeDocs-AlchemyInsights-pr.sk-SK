---
title: Obnovenie odstránenej lokality
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582250"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="84833-102">Obnovenie odstránenej lokality</span><span class="sxs-lookup"><span data-stu-id="84833-102">Restore a deleted site</span></span>

<span data-ttu-id="84833-103">Keď správca odstráni lokalitu SharePoint, umiestni sa do Koša kolekcie lokalít, kde sa uchováva 93 dní pred jej trvalým odstránením.</span><span class="sxs-lookup"><span data-stu-id="84833-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="84833-104">Obnovenie lokality:</span><span class="sxs-lookup"><span data-stu-id="84833-104">To restore the site:</span></span>
  
1. <span data-ttu-id="84833-105">V novom Centre spravovania služby SharePoint kliknite na páse s nástrojmi na položku **Kôš.**</span><span class="sxs-lookup"><span data-stu-id="84833-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="84833-106">Začiarknite políčko vedľa kolekcie lokalít, ktorú chcete obnoviť.</span><span class="sxs-lookup"><span data-stu-id="84833-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="84833-107">Kliknite na **položku Obnoviť odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="84833-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="84833-108">Ak chcete obnoviť odstránenú komunikačnú lokalitu, môžete použiť nové Centrum spravovania služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84833-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="84833-109">V opačnom prípade musíte použiť prostredie Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="84833-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="84833-110">Ak chcete obnoviť lokalitu, ktorá patrí do skupiny Microsoft 365, musíte obnoviť skupinu v Centre spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="84833-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="84833-111">Skupiny je možné obnoviť 30 dní po ich odstránení.</span><span class="sxs-lookup"><span data-stu-id="84833-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

