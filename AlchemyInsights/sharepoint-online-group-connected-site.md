---
title: Pridanie skupiny na lokalitu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771223"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="1ac0c-102">Problémy pri vytváraní skupiny pripojenej lokality v SharePointe</span><span class="sxs-lookup"><span data-stu-id="1ac0c-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="1ac0c-103">Niektoré bežné problémy, ktoré sa vyskytli pri vytváraní alebo opätovnom vytvorení lokality pripojenej k skupine.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="1ac0c-104">Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou URL adresou, budete musieť predchádzajúcu lokalitu odstrániť natrvalo.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="1ac0c-105">Stiahnuť [prostredie spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="1ac0c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="1ac0c-106">Ďalšie informácie o tom, ako začať pracovať s prostredím PowerShell, nájdete v téme Začíname [pracovať so službou SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="1ac0c-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="1ac0c-107">Odstránenie lokality z odstránených lokalít pomocou rutiny typu cmdlet prostredia na [Odstránenie SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="1ac0c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="1ac0c-108">Na trvalé odstránenie skupinových lokalít sa vyžaduje prostredie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="1ac0c-109">Ak vytvárate lokalitu pripojenú ku skupine a zobrazíte upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje**, pozrite si existujúce skupiny z [centra spravovania služby Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="1ac0c-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="1ac0c-110">Ak chcete problém vyriešiť, odstráňte existujúcu skupinu, ak ju už nepotrebujete, alebo vytvorte lokalitu s iným priradeným aliasom.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="1ac0c-111">Existujú rôzne spôsoby na vytváranie a používanie moderných skupín v SharePointe.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="1ac0c-112">Existujúce lokality môžete pripojiť k skupine Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1ac0c-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="1ac0c-113">Ďalšie informácie nájdete v téme [pripojenie skupiny Microsoft 365 pomocou používateľského rozhrania služby SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="1ac0c-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="1ac0c-114">Ak chcete vytvoriť lokalitu pripojenú ku skupine Microsoft 365, budete musieť vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="1ac0c-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
