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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582826"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="4b027-102">Problémy pri vytváraní skupiny pripojenej lokality v SharePointe</span><span class="sxs-lookup"><span data-stu-id="4b027-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="4b027-103">Pri vytváraní alebo opätovnom vytváraní skupiny pripojenej lokality sa vyskytli problémy.</span><span class="sxs-lookup"><span data-stu-id="4b027-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="4b027-104">Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou adresou URL, budete musieť natrvalo odstrániť predchádzajúcu lokalitu.</span><span class="sxs-lookup"><span data-stu-id="4b027-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="4b027-105">Stiahnuť [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="4b027-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="4b027-106">Ďalšie informácie o tom, ako začať pracovať s powershellom, nájdete v téme [Začíname pracovať s prostredím správy SharePointu Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="4b027-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="4b027-107">Odstránenie lokality z odstránených lokalít pomocou rutiny cmdlet prostredia Powershell [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="4b027-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="4b027-108">PowerShell je potrebné natrvalé odstránenie skupiny lokalít.</span><span class="sxs-lookup"><span data-stu-id="4b027-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="4b027-109">Ak vytvárate skupinu pripojenú lokalitu a zobrazí sa upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje,** skontrolujte existujúce skupiny z Centra spravovania služby [Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="4b027-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="4b027-110">Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.</span><span class="sxs-lookup"><span data-stu-id="4b027-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="4b027-111">Existujú rôzne spôsoby vytvárania a používania moderných skupín so SharePointom.</span><span class="sxs-lookup"><span data-stu-id="4b027-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="4b027-112">Existujúce lokality môžete pripojiť k skupine Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b027-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="4b027-113">Ďalšie informácie nájdete v téme [Pripojenie skupiny Microsoft 365 pomocou používateľského rozhrania SharePointu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="4b027-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="4b027-114">Ak chcete vytvoriť pripojenú lokalitu skupiny Microsoft 365, musíte vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="4b027-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
