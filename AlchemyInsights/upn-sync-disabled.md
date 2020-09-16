---
title: Synchronizácia hlavného mena používateľa je vypnutá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749529"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="4623e-102">Synchronizácia hlavného mena používateľa je vypnutá</span><span class="sxs-lookup"><span data-stu-id="4623e-102">UPN sync disabled</span></span>

<span data-ttu-id="4623e-103">Ak ste spustili synchronizáciu s Azúrovou REKLAMou pred 30. marca 2016, spustite nasledujúcu rutinu typu cmdlet prostredia PowerShell služby Azure AD, aby sa v organizácii povolila mäkká zhoda UPN len pre vašu organizáciu:</span><span class="sxs-lookup"><span data-stu-id="4623e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="4623e-104">**Set-MsolDirSyncFeature-funkcia EnableSoftMatchOnUpn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="4623e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="4623e-105">Funkcia UPN soft Match sa automaticky zapne pre organizácie, ktoré začali synchronizovať s Azúrovou REKLAMou alebo po 30. marci 2016.</span><span class="sxs-lookup"><span data-stu-id="4623e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="4623e-106">Ďalšie informácie o povolení funkcie soft Match v službách UPN a ďalších funkciách synchronizácie nájdete v téme [funkcie služby Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="4623e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

