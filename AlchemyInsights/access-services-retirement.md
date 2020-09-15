---
title: Prístup k dôchodkovým službám
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698697"
---
# <a name="access-services-retirement"></a><span data-ttu-id="61fd5-102">Prístup k dôchodkovým službám</span><span class="sxs-lookup"><span data-stu-id="61fd5-102">Access services retirement</span></span>

<span data-ttu-id="61fd5-103">Ako sme boli pôvodne vyhlásené v MC97576, v marci 2017 a pokračovali v komunikácii za uplynulý rok, v ktorom sú služby Accessu v dôchodku.</span><span class="sxs-lookup"><span data-stu-id="61fd5-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="61fd5-104">Ďalšou fázou v tomto procese bude odstránenie webových databáz Accessu, ktoré používajú zoznamy SharePointu ako základný ukladací priestor údajov.</span><span class="sxs-lookup"><span data-stu-id="61fd5-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="61fd5-105">**Ako to ovplyvní mňa?**</span><span class="sxs-lookup"><span data-stu-id="61fd5-105">**How does this affect me?**</span></span>

<span data-ttu-id="61fd5-106">Od júna 2019 sa ukončí vytváranie nových Accessových databáz v SharePointe Online a vypnutie služby a všetkých zostávajúcich aplikácií do apríla 2020.</span><span class="sxs-lookup"><span data-stu-id="61fd5-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="61fd5-107">**Čo je potrebné urobiť na prípravu tejto zmeny?**</span><span class="sxs-lookup"><span data-stu-id="61fd5-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="61fd5-108">Odporúčame vám vytvoriť plán prechodu pre webové databázy Accessu vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="61fd5-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="61fd5-109">Správcovia môžu použiť [skener aplikácie SharePoint Accessu](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) na získanie zoznamu prístupových aplikácií, ktoré lokality používajú.</span><span class="sxs-lookup"><span data-stu-id="61fd5-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="61fd5-110">Existuje niekoľko spôsobov migrácie údajov webových databáz Accessu:</span><span class="sxs-lookup"><span data-stu-id="61fd5-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="61fd5-111">Importuje sa do lokálnej Accessovej databázy (. ACCDB) alebo do excelového súboru.</span><span class="sxs-lookup"><span data-stu-id="61fd5-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="61fd5-112">Odporúčame tiež preskúmať Microsoft PowerApps ako alternatívnu platformu na vytváranie podnikových riešení bez kódu pre webové a mobilné zariadenia.</span><span class="sxs-lookup"><span data-stu-id="61fd5-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>