---
title: Vytvorenie lokality SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770870"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="52c41-102">Vytvorenie lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="52c41-102">Create a SharePoint site</span></span>

<span data-ttu-id="52c41-103">Vytvoriť alebo spravovať lokality z [aktívnych lokalít](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v stredisku SharePoint admin Center.</span><span class="sxs-lookup"><span data-stu-id="52c41-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="52c41-104">Ďalšie informácie nájdete v téme [spravovanie lokalít v novom centre spravovania služby SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="52c41-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="52c41-105">Tipy:</span><span class="sxs-lookup"><span data-stu-id="52c41-105">Tips:</span></span>

- <span data-ttu-id="52c41-106">**Nemôžete** vytvoriť lokalitu s rovnakou adresou URL existujúcej lokality.</span><span class="sxs-lookup"><span data-stu-id="52c41-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="52c41-107">Ak ste odstránili lokalitu a chcete znova použiť adresu URL, je možné, že odstránená lokalita stále existuje v časti [odstránené lokality](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="52c41-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="52c41-108">Lokalita sa bude musieť natrvalo odstrániť, aby opätovne používali adresu URL.</span><span class="sxs-lookup"><span data-stu-id="52c41-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="52c41-109">Ak chcete úplne odstrániť lokalitu pomocou prostredia PowerShell, pozrite si príklad rutiny cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="52c41-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="52c41-110">Niektorí používatelia nemusia byť schopní vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="52c41-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="52c41-111">[Pozrite si správa vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="52c41-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="52c41-112">Je možné, že stránka sa objaví prilepené na **Vytvorenie** dlhšie, než sa očakávalo.</span><span class="sxs-lookup"><span data-stu-id="52c41-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="52c41-113">Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste sa prosím lístok podpory.</span><span class="sxs-lookup"><span data-stu-id="52c41-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="52c41-114">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="52c41-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="52c41-115">Prosím, dajte nám aspoň 24 hodín na dokončenie riešenia.</span><span class="sxs-lookup"><span data-stu-id="52c41-115">Please give us at least 24 hours to complete a solution.</span></span>
