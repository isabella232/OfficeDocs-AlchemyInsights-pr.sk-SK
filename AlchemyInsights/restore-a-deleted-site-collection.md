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
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048811"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="65b3e-102">Obnovenie odstránenej lokality</span><span class="sxs-lookup"><span data-stu-id="65b3e-102">Restore a deleted site</span></span>

<span data-ttu-id="65b3e-103">Keď správca odstráni lokalitu SharePoint, umiestni sa do Koša kolekcie lokalít, kde sa uchováva 93 dní pred natrvalo odstrániť.</span><span class="sxs-lookup"><span data-stu-id="65b3e-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="65b3e-104">Obnovenie lokality:</span><span class="sxs-lookup"><span data-stu-id="65b3e-104">To restore the site:</span></span>
  
1. <span data-ttu-id="65b3e-105">V novom SharePoint admin Center, kliknite na tlačidlo **Kôš** na páse s nástrojmi.</span><span class="sxs-lookup"><span data-stu-id="65b3e-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="65b3e-106">Začiarknite políčko vedľa kolekcie lokalít, ktorú chcete obnoviť.</span><span class="sxs-lookup"><span data-stu-id="65b3e-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="65b3e-107">Kliknite na položku **obnoviť odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="65b3e-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="65b3e-108">Ak chcete obnoviť odstránenú komunikačnú lokalitu, môžete použiť nové centrum spravovania služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="65b3e-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="65b3e-109">V opačnom prípade musíte použiť prostredie Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="65b3e-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="65b3e-110">Ak chcete obnoviť lokalitu, ktorá patrí do skupiny Office 365, musíte obnoviť skupinu Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="65b3e-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="65b3e-111">Skupiny môžu byť obnovené po dobu 30 dní po ich odstránení.</span><span class="sxs-lookup"><span data-stu-id="65b3e-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

