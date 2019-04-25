---
title: Uložiť ako šablónu lokality alebo zoznamu
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243679"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="aecfd-102">Uložiť ako šablónu lokality alebo zoznamu</span><span class="sxs-lookup"><span data-stu-id="aecfd-102">Save site or list as a template</span></span>

<span data-ttu-id="aecfd-103">Šablóny lokality SharePoint sú predkompilované definície navrhnuté okolo konkrétnym pracovným požiadavkám.</span><span class="sxs-lookup"><span data-stu-id="aecfd-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="aecfd-104">Ďalšie informácie nájdete v téme [pomocou šablóny vytvoriť rôzne typy lokalít SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="aecfd-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="aecfd-105">Tu sú niektoré spoločné problémy/riešenia týkajúce sa uloženia lokality alebo zoznamu ako šablóny lokality SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="aecfd-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="aecfd-106">**Uložiť zoznam stránok šablóny tlačidlo je nie sú k dispozícii alebo chýbajúce**.</span><span class="sxs-lookup"><span data-stu-id="aecfd-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="aecfd-107">Správcovia musieť povoliť vlastné skript povoliť funkcie šablóny.</span><span class="sxs-lookup"><span data-stu-id="aecfd-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="aecfd-108">Podrobný postup, príklady a úvah nájdete [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="aecfd-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="aecfd-109">Uložiť lokalitu ako šablónu príkaz nie je podporovaný a môže spôsobiť problémy na webové stránky používajúce SharePoint Server Publishing infraštruktúry.</span><span class="sxs-lookup"><span data-stu-id="aecfd-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="aecfd-110">**Šablóna lokality sa nedá vytvoriť alebo nefunguje správne**</span><span class="sxs-lookup"><span data-stu-id="aecfd-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="aecfd-111">Šablóna môže byť chýbajúce [funkcie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje.</span><span class="sxs-lookup"><span data-stu-id="aecfd-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="aecfd-112">Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="aecfd-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="aecfd-113">Skontrolujte, ak žiadne zoznamy alebo knižnice prekročiť [Limit prah zobrazenia zoznamu](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže zablokovať vytvorenie šablóny lokality.</span><span class="sxs-lookup"><span data-stu-id="aecfd-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="aecfd-114">Lokality môžu používať príliš veľa prostriedkov a preto šablóna lokality presahuje limit 50 megabajtov (MB).</span><span class="sxs-lookup"><span data-stu-id="aecfd-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="aecfd-115">Tam sú problémy so zobrazovaním údajov zo zoznamu, ktorý používa vyhľadávacieho stĺpca.</span><span class="sxs-lookup"><span data-stu-id="aecfd-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="aecfd-116">Ďalšie informácie nájdete v téme [vytvorené šablóny zoznamu nezobrazuje údaje zo zoznamu správnu vyhľadávania SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="aecfd-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="aecfd-117">Pre podrobnejšie informácie o spoločných problémoch a riešeniach prosím odkaz, [Vytvorenie a používanie šablóny lokality](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="aecfd-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

