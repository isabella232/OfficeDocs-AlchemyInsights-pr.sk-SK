---
title: Prístup služieb dôchodkového
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495766"
---
# <a name="access-services-retirement"></a><span data-ttu-id="8dfe2-102">Prístup služieb dôchodkového</span><span class="sxs-lookup"><span data-stu-id="8dfe2-102">Access services retirement</span></span>

<span data-ttu-id="8dfe2-103">Ako sme pôvodne oznámená v MC97576, v marci 2017 a naďalej komunikovať v minulom roku prístup služby sú vyňatý z Office 365.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="8dfe2-104">Ďalšia fáza v tomto procese bude odstránenie prístupu Web databáz, ktoré používajú zoznamy SharePoint ako ich základný ukladací priestor údajov.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="8dfe2-105">**Ako ma to ovplyvní?**</span><span class="sxs-lookup"><span data-stu-id="8dfe2-105">**How does this affect me?**</span></span>

<span data-ttu-id="8dfe2-106">Od júna 2019, budeme zastaviť vytváranie nových databáz programu Access v službe SharePoint Online a vypnutie služby a všetky zostávajúce aplikácie do apríla roku 2020.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="8dfe2-107">**Čo je potrebné urobiť pre prípravu na túto zmenu?**</span><span class="sxs-lookup"><span data-stu-id="8dfe2-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="8dfe2-108">Odporúčame vám vytvoriť plán prechodu vaša organizácia prístup web databáz.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="8dfe2-109">Správcovia môžete použiť [SharePoint prístup app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získať súpis prístup aplikácií, ktoré stránky používajú.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="8dfe2-110">Existuje niekoľko spôsobov na migráciu údajov databáz web Access:</span><span class="sxs-lookup"><span data-stu-id="8dfe2-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="8dfe2-111">Import do lokálnej databázy Access (. ACCDB) alebo do súboru programu Excel.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="8dfe2-112">Odporúčame tiež skúmanie Microsoft PowerApps ako alternatívnu platformu vytvoriť bez kódu podnikové riešenia pre web a mobilné zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8dfe2-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>