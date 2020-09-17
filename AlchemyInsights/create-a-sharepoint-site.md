---
title: Vytvorenie lokality SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806954"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="6aad6-102">Vytvorenie lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="6aad6-102">Create a SharePoint site</span></span>

<span data-ttu-id="6aad6-103">Vytvárať alebo spravovať lokality z [aktívnych lokalít](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v centre spravovania služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6aad6-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="6aad6-104">Ďalšie informácie nájdete v téme [Správa lokalít v novom centre spravovania služby SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="6aad6-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="6aad6-105">Tipy</span><span class="sxs-lookup"><span data-stu-id="6aad6-105">Tips:</span></span>

- <span data-ttu-id="6aad6-106">**Nie je možné** vytvoriť lokalitu s rovnakou URL adresou existujúcej lokality.</span><span class="sxs-lookup"><span data-stu-id="6aad6-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="6aad6-107">Ak ste odstránili lokalitu a chcete ju znova použiť, je možné, že odstránená lokalita bude v časti [odstránené lokality](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)stále k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="6aad6-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="6aad6-108">Ak chcete znova použiť URL adresu, lokalita sa bude musieť natrvalo odstrániť.</span><span class="sxs-lookup"><span data-stu-id="6aad6-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="6aad6-109">Ak chcete úplne odstrániť lokalitu s prostredím PowerShell, pozrite si príklad rutiny typu cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="6aad6-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="6aad6-110">Niektorí používatelia pravdepodobne nebudú môcť vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="6aad6-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="6aad6-111">[Pozrite si tému správa vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="6aad6-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="6aad6-112">Je možné, že lokalita sa zobrazí prilepené na **Vytvorenie** dlhšieho, než sa očakávalo.</span><span class="sxs-lookup"><span data-stu-id="6aad6-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="6aad6-113">Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste lístok technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="6aad6-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="6aad6-114">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="6aad6-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6aad6-115">Ak chcete vyplniť riešenie, poskytnite nám aspoň 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="6aad6-115">Please give us at least 24 hours to complete a solution.</span></span>
