---
title: Vytvorenie lokality SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753723"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="53289-102">Vytvoriť pomocou šablóny lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="53289-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="53289-103">Šablóny lokality SharePoint sú predkompilované definície navrhnuté okolo konkrétnym pracovným požiadavkám.</span><span class="sxs-lookup"><span data-stu-id="53289-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="53289-104">Ďalšie informácie nájdete v téme [pomocou šablóny vytvoriť rôzne typy lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="53289-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="53289-105">Tu sú niektoré spoločné problémy/riešenia týkajúce sa uloženia lokality alebo zoznamu ako šablóny lokality Sharepoint online.</span><span class="sxs-lookup"><span data-stu-id="53289-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="53289-106">**Uložiť zoznam stránok šablóny tlačidlo nie je k dispozícii alebo chýbajúce**</span><span class="sxs-lookup"><span data-stu-id="53289-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="53289-107">Správcovia musieť povoliť vlastné skript povoliť funkcie šablóny.</span><span class="sxs-lookup"><span data-stu-id="53289-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="53289-108">Podrobný postup, pozrite si príklady a úvahy</span><span class="sxs-lookup"><span data-stu-id="53289-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="53289-109">Povolenie alebo zakázanie vlastný skript</span><span class="sxs-lookup"><span data-stu-id="53289-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="53289-110">Uložiť lokalitu ako šablónu príkaz nie je podporovaný a môže spôsobiť problémy na webové stránky používajúce SharePoint Server Publishing infraštruktúry.</span><span class="sxs-lookup"><span data-stu-id="53289-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="53289-111">Šablóna lokality sa nedá vytvoriť alebo nefunguje správne.</span><span class="sxs-lookup"><span data-stu-id="53289-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="53289-112">Šablóna môže byť chýbajúce [funkcie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje.</span><span class="sxs-lookup"><span data-stu-id="53289-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="53289-113">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="53289-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="53289-114">Skontrolujte, ak žiadne zoznamy alebo knižnice prekročiť [Limit prah zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže zablokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="53289-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="53289-115">Lokality môžu používať príliš veľa zdrojov a preto šablóna lokality prekračuje 50 MB limit.</span><span class="sxs-lookup"><span data-stu-id="53289-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="53289-116">Tam sú problémy so zobrazovaním údajov zo zoznamu, ktorý používa vyhľadávacieho stĺpca.</span><span class="sxs-lookup"><span data-stu-id="53289-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="53289-117">Ďalšie informácie nájdete v téme [vytvorené šablóny zoznamu nezobrazuje údaje zo zoznamu správnu vyhľadávania SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="53289-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="53289-118">Podrobnejšie informácie o spoločné problémy a riešenia, skontrolujte, či [Vytvorenie a používanie šablóny lokality](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="53289-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



