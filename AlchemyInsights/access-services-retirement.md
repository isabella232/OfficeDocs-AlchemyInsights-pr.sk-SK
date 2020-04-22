---
title: Prístup k službám odchod do dôchodku
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687273"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b452c-102">Prístup k službám odchod do dôchodku</span><span class="sxs-lookup"><span data-stu-id="b452c-102">Access services retirement</span></span>

<span data-ttu-id="b452c-103">Ako sme pôvodne oznámila v MC97576, v marci 2017, a pokračoval komunikovať za uplynulý rok prístup k službám sú v dôchodku.</span><span class="sxs-lookup"><span data-stu-id="b452c-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="b452c-104">Ďalšou fázou tohto procesu bude odstránenie webových databáz programu Access, ktoré používajú zoznamy lokality SharePoint ako ich základné úložisko údajov.</span><span class="sxs-lookup"><span data-stu-id="b452c-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b452c-105">**Ako to ovplyvní ma?**</span><span class="sxs-lookup"><span data-stu-id="b452c-105">**How does this affect me?**</span></span>

<span data-ttu-id="b452c-106">Od júna 2019, budeme zastaviť vytváranie nových databáz programu Access v SharePointe Online a vypnúť službu a všetky zostávajúce aplikácie do apríla 2020.</span><span class="sxs-lookup"><span data-stu-id="b452c-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b452c-107">**Čo potrebujem na to, aby ste sa pripravili na túto zmenu?**</span><span class="sxs-lookup"><span data-stu-id="b452c-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b452c-108">Odporúčame vám vytvoriť plán prechodu pre webové databázy programu Access vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="b452c-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="b452c-109">Správcovia môžu použiť [skener aplikácie SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) na získanie inventára prístupových aplikácií, ktoré lokality používajú.</span><span class="sxs-lookup"><span data-stu-id="b452c-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b452c-110">Existuje niekoľko spôsobov, ako migrovať údaje webových databáz programu Access:</span><span class="sxs-lookup"><span data-stu-id="b452c-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b452c-111">Importovanie do lokálnej databázy programu Access (. ACCDB) alebo do súboru programu Excel.</span><span class="sxs-lookup"><span data-stu-id="b452c-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b452c-112">Odporúčame tiež preskúmať službu Microsoft PowerApps ako alternatívnu platformu na vytvorenie podnikových riešení bez kódu pre webové a mobilné zariadenia.</span><span class="sxs-lookup"><span data-stu-id="b452c-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>