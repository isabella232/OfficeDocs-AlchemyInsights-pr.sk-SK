---
title: Pracovný postup sa nezačína
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794782"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="05622-102">Pracovný postup sa nezačína</span><span class="sxs-lookup"><span data-stu-id="05622-102">Workflow is not starting</span></span>

- <span data-ttu-id="05622-103">Pracovné postupy SharePointu 2010 a SharePointu 2013 sa nespúšťajú.</span><span class="sxs-lookup"><span data-stu-id="05622-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="05622-104">Ak sa váš pracovný postup nespúšťa, môže sa vyskytnúť dočasný problém so službou, v ktorom sa môžu používatelia občas zdržiavať s priebehom pracovného postupu.</span><span class="sxs-lookup"><span data-stu-id="05622-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="05622-105">Ak chcete zistiť, či je vaša organizácia ovplyvnená, pozrite si [tabuľu stavu služby](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="05622-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="05622-106">Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste lístok technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="05622-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="05622-107">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="05622-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="05622-108">Ak chcete vyplniť riešenie, poskytnite nám aspoň 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="05622-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="05622-109">Pracovné postupy SharePointu 2010 oneskorené pri spustení.</span><span class="sxs-lookup"><span data-stu-id="05622-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="05622-110">Tento problém sa vyskytuje, ak je pracovný postup spustený vo veľkých dávkach.</span><span class="sxs-lookup"><span data-stu-id="05622-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="05622-111">(napríklad pri pridávaní viacerých položiek naraz).</span><span class="sxs-lookup"><span data-stu-id="05622-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="05622-112">Pracovné postupy nie sú určené na spustenie v reálnom čase, takže oneskorenie je pri návrhu.</span><span class="sxs-lookup"><span data-stu-id="05622-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="05622-113">Ak je pracovný postup zložitý Extensible Object Markup Language (XMOL), kompilácia môže byť pomalý.</span><span class="sxs-lookup"><span data-stu-id="05622-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="05622-114">Pozrite si [Tento](https://support.microsoft.com//kb/3043697) článok.</span><span class="sxs-lookup"><span data-stu-id="05622-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="05622-115">Pracovný postup by ste mali zjednodušiť alebo ho môžete znova navrhnúť pomocou typu platformy pracovného postupu Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="05622-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="05622-116">Ak sa História pracovných postupov rozrástla na veľké, možno budete chcieť vyčistiť položky alebo vytvoriť nový zoznam histórie.</span><span class="sxs-lookup"><span data-stu-id="05622-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="05622-117">Ďalšie informácie: [Vymazanie histórie pracovného postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="05622-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="05622-118">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="05622-118">Related topics</span></span>
<span data-ttu-id="05622-119">Chcete vyskúšať Microsoft flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="05622-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="05622-120">Vytvorenie toku</span><span class="sxs-lookup"><span data-stu-id="05622-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="05622-121">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="05622-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


