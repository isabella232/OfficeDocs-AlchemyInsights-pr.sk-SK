---
title: Vytvorenie lokality SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755323"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="17ebd-102">Vytvorenie lokalít SharePoint pomocou šablón</span><span class="sxs-lookup"><span data-stu-id="17ebd-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="17ebd-103">Šablóny lokality SharePoint sú vopred zostavené definície navrhnuté okolo konkrétnej obchodnej potreby.</span><span class="sxs-lookup"><span data-stu-id="17ebd-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="17ebd-104">Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych typov lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="17ebd-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="17ebd-105">Tu sú niektoré bežné problémy alebo riešenia týkajúce sa ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="17ebd-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="17ebd-106">**Tlačidlo Uložiť stránku alebo šablónu zoznamu nie je k dispozícii alebo chýba**</span><span class="sxs-lookup"><span data-stu-id="17ebd-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="17ebd-107">Správcovia budú musieť povoliť vlastný skript, aby šablóny funkcie.</span><span class="sxs-lookup"><span data-stu-id="17ebd-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="17ebd-108">Podrobné kroky, príklady a úvahy nájdete v časti</span><span class="sxs-lookup"><span data-stu-id="17ebd-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="17ebd-109">Povolenie alebo zabránenie prispôsobeniu skriptu</span><span class="sxs-lookup"><span data-stu-id="17ebd-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="17ebd-110">Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobiť problémy na lokalitách, ktoré používajú SharePoint Server publikovanie infraštruktúry.</span><span class="sxs-lookup"><span data-stu-id="17ebd-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="17ebd-111">**Šablóna lokality sa nedá vytvoriť alebo nepracuje správne**</span><span class="sxs-lookup"><span data-stu-id="17ebd-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="17ebd-112">Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nebude sa aktivovať.</span><span class="sxs-lookup"><span data-stu-id="17ebd-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="17ebd-113">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.</span><span class="sxs-lookup"><span data-stu-id="17ebd-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="17ebd-114">Skontrolujte, či zoznamy alebo knižnice presahujú [limit limitu zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="17ebd-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="17ebd-115">Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality presahuje limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="17ebd-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="17ebd-116">Existujú problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec.</span><span class="sxs-lookup"><span data-stu-id="17ebd-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="17ebd-117">Ďalšie informácie nájdete v časti [zoznam vygenerovaný šablónou nezobrazuje údaje zo správneho vyhľadávacieho zoznamu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="17ebd-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="17ebd-118">Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v téme [Vytvorenie a používanie šablón lokality](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="17ebd-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



