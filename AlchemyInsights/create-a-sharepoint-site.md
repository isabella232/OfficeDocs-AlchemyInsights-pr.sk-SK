---
title: Vytvorenie lokality SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802981"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="e03ac-102">Vytvorenie lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="e03ac-102">Create a SharePoint site</span></span>

<span data-ttu-id="e03ac-103">Môžete vidieť tieto informácie o vytvorenie lokality SharePoint:</span><span class="sxs-lookup"><span data-stu-id="e03ac-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="e03ac-104">[Spravovanie lokalít v nových SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): dozvedieť sa o možnosti vytvorenia lokality, vrátane ako vytvoriť klasické tímy lokalitu alebo že neobsahuje skupiny Office 365.</span><span class="sxs-lookup"><span data-stu-id="e03ac-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="e03ac-105">[Vytvorenie tímovej lokality SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Naučte sa vytvoriť lokalitu tímu.</span><span class="sxs-lookup"><span data-stu-id="e03ac-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="e03ac-106">[Vytvoriť oznámenie lokality SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Naučte sa vytvoriť lokalitu komunikácií.</span><span class="sxs-lookup"><span data-stu-id="e03ac-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="e03ac-107">[Spravovanie lokalít v nových SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Naučte sa vytvoriť klasické miesto alebo tímovej lokality, ktorý neobsahuje skupiny Office 365.</span><span class="sxs-lookup"><span data-stu-id="e03ac-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tipy]
> - <span data-ttu-id="e03ac-109">Nemôžete vytvoriť stránky na rovnakej adrese URL existujúcej lokality.</span><span class="sxs-lookup"><span data-stu-id="e03ac-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="e03ac-110">Ak odstránené stránky a chcú znovu použiť URL, je možné odstránené lokalít stále existuje pod **Odstránené stránky**.</span><span class="sxs-lookup"><span data-stu-id="e03ac-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="e03ac-111">Spravovať odstránené lokalít, pozrite [Odstránenie lokality](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="e03ac-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="e03ac-112">Úplné odstránenie lokality pomocou prostredia Powershell, pozri príklad cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="e03ac-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="e03ac-113">Niektorí používatelia možno nebudú schopní vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="e03ac-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="e03ac-114">Pozrite si [Vytvorenie spravovať lokality SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="e03ac-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="e03ac-115">Je možné, stránky sa zobrazí ponechané na **vytváranie** dlhšie, než sa očakávalo.</span><span class="sxs-lookup"><span data-stu-id="e03ac-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="e03ac-116">Ak uplynulo viac ako 24 hodín od najprv ste videli tento problém, prihláste sa prosím na podporu lístok.</span><span class="sxs-lookup"><span data-stu-id="e03ac-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e03ac-117">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="e03ac-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e03ac-118">Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.</span><span class="sxs-lookup"><span data-stu-id="e03ac-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="e03ac-119">Ak potrebujete vytvoriť novú tímovú lokalitu, ktorá neobsahuje skupiny Office 365,</span><span class="sxs-lookup"><span data-stu-id="e03ac-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


