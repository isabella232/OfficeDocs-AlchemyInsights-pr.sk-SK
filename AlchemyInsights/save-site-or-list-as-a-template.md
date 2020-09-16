---
title: Uloženie lokality alebo zoznamu ako šablóny
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727546"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="8f6f5-102">Uloženie lokality alebo zoznamu ako šablóny</span><span class="sxs-lookup"><span data-stu-id="8f6f5-102">Save site or list as a template</span></span>

<span data-ttu-id="8f6f5-103">Šablóny lokality SharePoint sú vopred definované definície navrhnuté okolo konkrétnej podnikovej potreby.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8f6f5-104">Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych druhov lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8f6f5-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8f6f5-105">Tu je niekoľko bežných problémov a riešení, ktoré sa týkajú ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="8f6f5-106">**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba**.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="8f6f5-107">Správcovia budú musieť povoliť vlastné skripty na povolenie funkcií šablón.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8f6f5-108">Podrobné kroky, príklady a poznámky nájdete v téme [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8f6f5-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="8f6f5-109">Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobovať problémy na lokalitách, v ktorých sa používa Infraštruktúra publikovania servera SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="8f6f5-110">**Šablónu lokality nie je možné vytvoriť alebo nefunguje správne**</span><span class="sxs-lookup"><span data-stu-id="8f6f5-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="8f6f5-111">Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nedá sa aktivovať.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="8f6f5-112">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="8f6f5-113">Skontrolujte, či niektoré zoznamy alebo knižnice presiahnu [limitné hodnoty zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="8f6f5-114">Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality prekračuje limit 50 megabajtov (MB).</span><span class="sxs-lookup"><span data-stu-id="8f6f5-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="8f6f5-115">Vyskytli sa problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec.</span><span class="sxs-lookup"><span data-stu-id="8f6f5-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8f6f5-116">Ďalšie informácie nájdete v téme [zoznam generovaný šablónou sa nezobrazujú údaje zo správneho vyhľadávacieho zoznamu v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="8f6f5-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="8f6f5-117">Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v odkaze na [Vytvorenie a použitie šablón lokalít](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="8f6f5-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

