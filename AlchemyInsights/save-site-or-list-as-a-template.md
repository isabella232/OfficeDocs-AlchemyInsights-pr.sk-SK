---
title: Uložiť lokalitu alebo zoznam ako šablónu
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752047"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="3d975-102">Uložiť lokalitu alebo zoznam ako šablónu</span><span class="sxs-lookup"><span data-stu-id="3d975-102">Save site or list as a template</span></span>

<span data-ttu-id="3d975-103">Šablóny lokality SharePoint sú vopred zostavené definície navrhnuté okolo konkrétnej obchodnej potreby.</span><span class="sxs-lookup"><span data-stu-id="3d975-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="3d975-104">Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych typov lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="3d975-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="3d975-105">Tu sú niektoré bežné problémy alebo riešenia týkajúce sa ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="3d975-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="3d975-106">**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba**.</span><span class="sxs-lookup"><span data-stu-id="3d975-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="3d975-107">Správcovia budú musieť povoliť vlastný skript, aby šablóny funkcie.</span><span class="sxs-lookup"><span data-stu-id="3d975-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3d975-108">Podrobné kroky, príklady a úvahy nájdete v téme [povolenie alebo zabránenie prispôsobeniu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="3d975-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="3d975-109">Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobiť problémy na lokalitách, ktoré používajú SharePoint Server publikovanie infraštruktúry.</span><span class="sxs-lookup"><span data-stu-id="3d975-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="3d975-110">**Šablóna lokality sa nedá vytvoriť alebo nepracuje správne**</span><span class="sxs-lookup"><span data-stu-id="3d975-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="3d975-111">Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nebude sa aktivovať.</span><span class="sxs-lookup"><span data-stu-id="3d975-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="3d975-112">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.</span><span class="sxs-lookup"><span data-stu-id="3d975-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="3d975-113">Skontrolujte, či zoznamy alebo knižnice presahujú [limit limitu zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="3d975-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="3d975-114">Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality presahuje limit 50 megabajt (MB).</span><span class="sxs-lookup"><span data-stu-id="3d975-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="3d975-115">Existujú problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec.</span><span class="sxs-lookup"><span data-stu-id="3d975-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3d975-116">Ďalšie informácie nájdete v časti [zoznam vygenerovaný šablónou nezobrazuje údaje zo správneho vyhľadávacieho zoznamu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="3d975-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="3d975-117">Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v referencia, [vytváranie a používanie šablón stránok](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3d975-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

