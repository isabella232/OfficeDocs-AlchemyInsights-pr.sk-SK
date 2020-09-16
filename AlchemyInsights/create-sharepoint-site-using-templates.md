---
title: Vytvorenie lokality v SharePointe Online
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
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732254"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="77bc3-102">Vytvorenie lokalít SharePoint pomocou šablón</span><span class="sxs-lookup"><span data-stu-id="77bc3-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="77bc3-103">Možnosť Uložiť lokalitu ako šablónu nie je podporovaná s modernou komunikačnou lokalitou alebo tímovými lokalitami.</span><span class="sxs-lookup"><span data-stu-id="77bc3-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="77bc3-104">Ďalšie informácie o používaní šablón nájdete v téme [Uloženie, stiahnutie a nahratie lokality SharePoint ako šablóny](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="77bc3-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="77bc3-105">Tu je niekoľko bežných problémov a riešení, ktoré sa týkajú ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="77bc3-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="77bc3-106">**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba**</span><span class="sxs-lookup"><span data-stu-id="77bc3-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="77bc3-107">Správcovia budú musieť povoliť vlastné skripty na povolenie funkcií šablón.</span><span class="sxs-lookup"><span data-stu-id="77bc3-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="77bc3-108">Podrobné kroky, príklady a poznámky nájdete v téme</span><span class="sxs-lookup"><span data-stu-id="77bc3-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="77bc3-109">Povolenie alebo zakázanie vlastného skriptu</span><span class="sxs-lookup"><span data-stu-id="77bc3-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="77bc3-110">Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobovať problémy na lokalitách, v ktorých sa používa Infraštruktúra publikovania servera SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="77bc3-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="77bc3-111">**Šablónu lokality nie je možné vytvoriť alebo nefunguje správne**</span><span class="sxs-lookup"><span data-stu-id="77bc3-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="77bc3-112">Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nedá sa aktivovať.</span><span class="sxs-lookup"><span data-stu-id="77bc3-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="77bc3-113">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.</span><span class="sxs-lookup"><span data-stu-id="77bc3-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="77bc3-114">Skontrolujte, či niektoré zoznamy alebo knižnice presiahnu [limitné hodnoty zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="77bc3-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="77bc3-115">Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality prekračuje limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="77bc3-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="77bc3-116">Vyskytli sa problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec.</span><span class="sxs-lookup"><span data-stu-id="77bc3-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="77bc3-117">Ďalšie informácie nájdete v téme [zoznam generovaný šablónou sa nezobrazujú údaje zo správneho vyhľadávacieho zoznamu v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="77bc3-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="77bc3-118">Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v políčka [Vytvorenie a používanie šablón lokalít](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="77bc3-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



