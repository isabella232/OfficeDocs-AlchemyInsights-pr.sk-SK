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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051116"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="8d11b-102">Problémy pri vytváraní alebo zoskupovanie pripojených lokalít SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8d11b-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="8d11b-103">Existuje niekoľko bežných problémov, ktoré sa vyskytli pri vytváraní alebo opätovnom vytvorení skupiny pripojenej lokality.</span><span class="sxs-lookup"><span data-stu-id="8d11b-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="8d11b-104">Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou webovou adresou, musíte natrvalo odstrániť predchádzajúcu lokalitu.</span><span class="sxs-lookup"><span data-stu-id="8d11b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="8d11b-105">Na stiahnutie [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="8d11b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="8d11b-106">Ďalšie informácie o Začíname s PowerShell, pozrite si Začíname [s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="8d11b-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="8d11b-107">Odstráňte lokalitu z odstránených lokalít pomocou rutiny cmdlet prostredia PowerShell [odstrániť SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="8d11b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="8d11b-108">Ak vytvárate skupinu pripojenú lokalitu a prijmete upozornenie, ďalšia skupina s rovnakým aliasom už existuje, skontrolujte existujúce skupiny z [balíka Office 365 z centra spravovania](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="8d11b-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="8d11b-109">Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.</span><span class="sxs-lookup"><span data-stu-id="8d11b-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="8d11b-110">Existujú rôzne spôsoby vytvárania a používania moderných skupín so službou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d11b-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="8d11b-111">Existujúce lokality môžete pripojiť k skupine Office 365.</span><span class="sxs-lookup"><span data-stu-id="8d11b-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="8d11b-112">Ďalšie informácie nájdete v téme [pripojenie skupiny Office 365 pomocou používateľa služby SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="8d11b-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="8d11b-113">Ak chcete vytvoriť lokalitu Connected Office 365 Group, musíte vytvoriť tímovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="8d11b-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="8d11b-114">Ďalšie informácie nájdete v téme [vytvorenie tímovej lokality v službe SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="8d11b-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

