---
title: Obnovenie odstránenej lokality
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692058"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="2be66-102">Obnovenie odstránenej lokality</span><span class="sxs-lookup"><span data-stu-id="2be66-102">Restore a deleted site</span></span>

<span data-ttu-id="2be66-103">Keď správca odstráni lokalitu SharePoint, umiestni sa do Koša kolekcie lokalít, kde sa uchová v priebehu 93 dní, kým sa natrvalo odstráni.</span><span class="sxs-lookup"><span data-stu-id="2be66-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="2be66-104">Obnovenie lokality:</span><span class="sxs-lookup"><span data-stu-id="2be66-104">To restore the site:</span></span>
  
1. <span data-ttu-id="2be66-105">V novom centre spravovania služby SharePoint kliknite na položku **Kôš** na páse s nástrojmi.</span><span class="sxs-lookup"><span data-stu-id="2be66-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="2be66-106">Začiarknite políčko vedľa kolekcie lokalít, ktorú chcete obnoviť.</span><span class="sxs-lookup"><span data-stu-id="2be66-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="2be66-107">Kliknite na položku **obnoviť odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="2be66-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="2be66-108">Ak chcete obnoviť odstránenú komunikačnú lokalitu, môžete použiť nové centrum spravovania služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2be66-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="2be66-109">V opačnom prípade je potrebné použiť prostredie Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2be66-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="2be66-110">Ak chcete obnoviť lokalitu, ktorá patrí do skupiny Microsoft 365, musíte skupinu obnoviť v centre spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="2be66-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="2be66-111">Skupiny je možné obnoviť po uplynutí 30 dní po odstránení.</span><span class="sxs-lookup"><span data-stu-id="2be66-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

