---
title: Vytvorenie lokality SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769606"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="9308e-102">Vytvorenie lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="9308e-102">Create a SharePoint site</span></span>

<span data-ttu-id="9308e-103">Informácie o vytváraní lokality SharePoint nájdete v nasledujúcich témach:</span><span class="sxs-lookup"><span data-stu-id="9308e-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="9308e-104">[Spravovanie lokalít v novom centre spravovania služby SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): informácie o možnostiach vytvárania lokalít vrátane vytvorenia klasickej lokality alebo tímového webu, ktorý nezahŕňa skupinu Office 365.</span><span class="sxs-lookup"><span data-stu-id="9308e-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="9308e-105">[Vytvorenie tímovej lokality v SharePointe](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Naučte sa vytvoriť tímovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="9308e-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="9308e-106">[Vytvorenie komunikačnej lokality v SharePointe Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Naučte sa vytvoriť komunikačnú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="9308e-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="9308e-107">[Spravovanie lokalít v novom centre spravovania služby SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Naučte sa vytvoriť klasickú lokalitu alebo tímovú lokalitu, ktorá nezahŕňa skupinu Office 365.</span><span class="sxs-lookup"><span data-stu-id="9308e-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="9308e-108">**Tipy:**</span><span class="sxs-lookup"><span data-stu-id="9308e-108">**Tips:**</span></span>
- <span data-ttu-id="9308e-109">Nemôžete vytvoriť lokalitu s rovnakou adresou URL existujúcej lokality.</span><span class="sxs-lookup"><span data-stu-id="9308e-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="9308e-110">Ak ste odstránili lokalitu a chcete znova použiť adresu URL, je možné, že odstránená lokalita stále existuje v časti **odstránené lokality**.</span><span class="sxs-lookup"><span data-stu-id="9308e-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="9308e-111">Ak chcete správu odstránených lokalít Zobraziť, [odstráňte lokalitu](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="9308e-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="9308e-112">Ak chcete úplne odstrániť lokalitu pomocou prostredia PowerShell, pozrite si príklad rutiny cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="9308e-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="9308e-113">Niektorí používatelia nemusia byť schopní vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="9308e-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="9308e-114">Pozrite si [Správa vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="9308e-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="9308e-115">Je možné, že stránka sa objaví prilepené na **Vytvorenie** dlhšie, než sa očakávalo.</span><span class="sxs-lookup"><span data-stu-id="9308e-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="9308e-116">Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste sa prosím lístok podpory.</span><span class="sxs-lookup"><span data-stu-id="9308e-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9308e-117">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="9308e-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9308e-118">Prosím, dajte nám aspoň 24 hodín na dokončenie riešenia.</span><span class="sxs-lookup"><span data-stu-id="9308e-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="9308e-119">Ak potrebujete vytvoriť novú tímovú lokalitu, ktorá nezahŕňa skupinu Office 365,</span><span class="sxs-lookup"><span data-stu-id="9308e-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


