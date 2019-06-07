---
title: Pridať skupinu lokality SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758745"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="3c6b6-102">Vytvorenie skupiny pripojené lokality SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3c6b6-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="3c6b6-103">Existuje niekoľko spoločných otázok sa vyskytla vytvorenie alebo re-vytvárať skupinu pripojení stránky.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="3c6b6-104">Ak ste odstránili skupine a jej prepojené stránky a chcete vytvoriť inú stránku s rovnakou adresou URL, musíte natrvalo odstrániť predchádzajúcu stránku.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="3c6b6-105">Stiahnuť [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="3c6b6-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="3c6b6-106">Viac info na Začíname s powershell v téme [Začíname pracovať s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="3c6b6-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="3c6b6-107">Odstránenie lokality zo odstránené lokalít pomocou rutiny cmdlet [Remove-SPODeletedSiteSharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) prostredia powershell.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="3c6b6-108">Ak vytvárate skupina prepojených stránok a upozornení, iné skupiny s rovnakým aliasu už existuje, skontrolujte, či existujúce skupiny z [Office 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="3c6b6-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="3c6b6-109">Ak chcete vyriešiť problém, ak už nie je potrebné odstrániť existujúcu skupinu alebo vytvoríte stránky s rozdielnymi aliasmi pridelené.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="3c6b6-110">Existujú rôzne spôsoby, ako vytvoriť a používať moderné skupiny so službou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="3c6b6-111">Existujúce lokality môžete pripojiť do skupiny Office 365.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="3c6b6-112">Ďalšie informácie nájdete v téme [pripojenie skupiny Office 365 pomocou SharePoint používateľa ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="3c6b6-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="3c6b6-113">Ak chcete vytvoriť lokalitu Office 365 skupiny pripojené, budete musieť vytvoriť lokalitu tímu.</span><span class="sxs-lookup"><span data-stu-id="3c6b6-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="3c6b6-114">Ďalšie informácie nájdete v téme [vytvorenie tímovej lokality SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="3c6b6-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

