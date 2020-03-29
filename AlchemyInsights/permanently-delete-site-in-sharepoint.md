---
title: Trvalé odstránenie lokality v SharePointe
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955238"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="6e794-102">Trvalé odstránenie lokality v SharePointe</span><span class="sxs-lookup"><span data-stu-id="6e794-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="6e794-103">Ak chcete znova použiť URL adresu z odstránenej lokality (na opätovné vytvorenie lokality) alebo natrvalo odstrániť lokalitu, pretože sa už nepoužíva, môžete použiť príkaz **Natrvalo odstrániť** v novom centre spravovania SharePointu.</span><span class="sxs-lookup"><span data-stu-id="6e794-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="6e794-104">Prejdite na [stránku Odstránené lokality v novom centre spravovania SharePointu](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) a prihláste sa pomocou konta, ktoré má povolenia správcu pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="6e794-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="6e794-105">V ľavom stĺpci vyberte lokalitu.</span><span class="sxs-lookup"><span data-stu-id="6e794-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="6e794-106">Kliknite na položku **Natrvalo odstrániť**.</span><span class="sxs-lookup"><span data-stu-id="6e794-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="6e794-107">**Poznámka**: Lokality pripojené k skupine nie je možné natrvalo odstrániť v novom centre spravovania SharePointu.</span><span class="sxs-lookup"><span data-stu-id="6e794-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="6e794-108">Namiesto toho sa musí použiť príkaz [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="6e794-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="6e794-109">Ďalšie informácie sú uvedené v článku [Trvalé odstránenie lokality](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="6e794-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
