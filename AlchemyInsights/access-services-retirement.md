---
title: Prístup služieb dôchodkového
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973948"
---
# <a name="access-services-retirement"></a><span data-ttu-id="ebe4f-102">Prístup služieb dôchodkového</span><span class="sxs-lookup"><span data-stu-id="ebe4f-102">Access services retirement</span></span>

<span data-ttu-id="ebe4f-103">Ako sme pôvodne oznámená v MC97576, v marci 2017 a naďalej komunikovať v minulom roku prístup služby sú vyňatý z Office 365.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="ebe4f-104">Ďalšia fáza v tomto procese bude odstránenie prístupu Web databáz, ktoré používajú zoznamy SharePoint ako ich základný ukladací priestor údajov.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="ebe4f-105">Ako ma to ovplyvní?</span><span class="sxs-lookup"><span data-stu-id="ebe4f-105">How does this affect me?</span></span>

<span data-ttu-id="ebe4f-106">Od júna 2019, budeme zastaviť vytváranie nových databáz programu Access v službe SharePoint Online a vypnutie služby a všetky zostávajúce aplikácie do apríla roku 2020.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="ebe4f-107">Čo je potrebné urobiť pre prípravu na túto zmenu?</span><span class="sxs-lookup"><span data-stu-id="ebe4f-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="ebe4f-108">Odporúčame vám vytvoriť plán prechodu vaša organizácia prístup web databáz.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="ebe4f-109">Správcovia môžete použiť [SharePoint prístup app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) získať súpis prístup aplikácií, ktoré stránky používajú.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="ebe4f-110">Existuje niekoľko spôsobov na migráciu údajov databáz web Access:</span><span class="sxs-lookup"><span data-stu-id="ebe4f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="ebe4f-111">Import do lokálnej databázy Access (. ACCDB) alebo do súboru programu Excel.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="ebe4f-112">Odporúčame tiež skúmanie Microsoft PowerApps ako alternatívnu platformu vytvoriť bez kódu podnikové riešenia pre web a mobilné zariadenia.</span><span class="sxs-lookup"><span data-stu-id="ebe4f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>