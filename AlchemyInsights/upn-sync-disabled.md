---
title: UPN synchronizácia zdravotne postihnutých
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311749"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="58e58-102">UPN synchronizácia zdravotne postihnutých</span><span class="sxs-lookup"><span data-stu-id="58e58-102">UPN sync disabled</span></span>

<span data-ttu-id="58e58-103">Ak ste začali synchronizácii Azure AD pred marca 30, 2016, spustiť nasledovné cmdlet Azure AD PowerShell umožniť UPN mäkké zápas pre vašu organizáciu len:</span><span class="sxs-lookup"><span data-stu-id="58e58-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="58e58-104">**Set-MsolDirSyncFeature-majú EnableSoftMatchOnUpn-povoliť $True**</span><span class="sxs-lookup"><span data-stu-id="58e58-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="58e58-105">UPN mäkké match sa automaticky zapne pre organizácie, ktoré začali synchronizácie s azúrovo reklamy alebo po marec 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="58e58-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="58e58-106">Ďalšie informácie o zapnutí mäkké zápas na UPN a ďalšie funkcie synchronizácie, nájdete [Azure AD pripojiť funkcie synchronizácie služby](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="58e58-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

