---
title: UPN Sync zakázané
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726119"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="d90a1-102">UPN Sync zakázané</span><span class="sxs-lookup"><span data-stu-id="d90a1-102">UPN sync disabled</span></span>

<span data-ttu-id="d90a1-103">Ak ste spustili synchronizáciu Azure AD pred marec 30, 2016, spustite nasledujúce rutiny cmdlet Azure AD PowerShell umožniť UPN soft Match len pre vašu organizáciu:</span><span class="sxs-lookup"><span data-stu-id="d90a1-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="d90a1-104">**Súbor MsolDirSyncFeature-funkcia EnableSoftMatchOnUpn-povoliť $True**</span><span class="sxs-lookup"><span data-stu-id="d90a1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="d90a1-105">UPN soft Match je automaticky zapnutá pre organizácie, ktoré začali synchronizáciu Azure AD alebo po marec 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="d90a1-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="d90a1-106">Ďalšie informácie o zapnutí funkcie soft Match v UPN a ďalších funkciách synchronizácie nájdete v časti [funkcie služby Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="d90a1-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

