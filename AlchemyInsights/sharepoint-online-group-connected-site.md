---
title: Pridanie skupiny na lokalitu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770366"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="2d6a7-102">Problémy pri vytváraní skupiny pripojenej lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="2d6a7-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="2d6a7-103">Niektoré bežné problémy sa vyskytli pri vytváraní alebo opätovnom vytvorení skupiny pripojenej lokality.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="2d6a7-104">Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou webovou adresou, musíte natrvalo odstrániť predchádzajúcu lokalitu.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="2d6a7-105">Na stiahnutie [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="2d6a7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="2d6a7-106">Ďalšie informácie o Začíname s PowerShell, pozrite si Začíname [s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="2d6a7-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="2d6a7-107">Odstráňte lokalitu z odstránených lokalít pomocou rutiny cmdlet prostredia PowerShell [odstrániť SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="2d6a7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="2d6a7-108">PowerShell je potrebné natrvalo odstrániť skupiny lokalít.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="2d6a7-109">Ak vytvárate skupinu pripojenú lokalitu a prijmete upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje**, skontrolujte existujúce skupiny z [balíka Office 365 z centrum spravovania](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="2d6a7-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="2d6a7-110">Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="2d6a7-111">Existujú rôzne spôsoby vytvárania a používania moderných skupín so službou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="2d6a7-112">Existujúce lokality môžete pripojiť k skupine Office 365.</span><span class="sxs-lookup"><span data-stu-id="2d6a7-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="2d6a7-113">Ďalšie informácie nájdete v téme [pripojenie skupiny Office 365 pomocou používateľského rozhrania služby SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="2d6a7-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="2d6a7-114">Ak chcete vytvoriť lokalitu Connected Office 365 Group, musíte vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="2d6a7-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
