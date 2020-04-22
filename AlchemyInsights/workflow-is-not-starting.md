---
title: Pracovný postup sa nespúšťa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766112"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b626d-102">Pracovný postup sa nespúšťa</span><span class="sxs-lookup"><span data-stu-id="b626d-102">Workflow is not starting</span></span>

- <span data-ttu-id="b626d-103">SharePoint 2010 a SharePoint 2013 toky činností sa nespúšťa.</span><span class="sxs-lookup"><span data-stu-id="b626d-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b626d-104">Ak váš pracovný postup nie je začína, môže existovať dočasný problém služby, kde používatelia môžu vyskytnúť občasné oneskorenie s workflow pokrok.</span><span class="sxs-lookup"><span data-stu-id="b626d-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b626d-105">Ak chcete zistiť, či je vaša organizácia ovplyvnená, skontrolujte [stav služby](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="b626d-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b626d-106">Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste sa prosím lístok podpory.</span><span class="sxs-lookup"><span data-stu-id="b626d-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b626d-107">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="b626d-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b626d-108">Prosím, dajte nám aspoň 24 hodín na dokončenie riešenia.</span><span class="sxs-lookup"><span data-stu-id="b626d-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b626d-109">SharePoint 2010 pracovné postupy oneskorené na začiatku.</span><span class="sxs-lookup"><span data-stu-id="b626d-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b626d-110">To nastane, ak pracovný postup sa spúšťa vo veľkých dávkach.</span><span class="sxs-lookup"><span data-stu-id="b626d-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b626d-111">(napríklad pri pridaní viacerých položiek naraz).</span><span class="sxs-lookup"><span data-stu-id="b626d-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b626d-112">Pracovné postupy nie sú určené na spustenie v reálnom čase, takže oneskorenie je podľa-Design správanie.</span><span class="sxs-lookup"><span data-stu-id="b626d-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b626d-113">Ak je pracovný postup zložitý Extensible Object Markup Language (XMOL), kompilácia môže byť pomalé.</span><span class="sxs-lookup"><span data-stu-id="b626d-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b626d-114">Pozrite si [Tento](https://support.microsoft.com//kb/3043697) článok.</span><span class="sxs-lookup"><span data-stu-id="b626d-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b626d-115">Pracovný postup by ste mali zjednodušiť alebo ho môžete prepracovať pomocou typu platformy Microsoft SharePoint 2013 workflow.</span><span class="sxs-lookup"><span data-stu-id="b626d-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b626d-116">Ak sa História pracovného postupu rozrástla veľké, možno budete chcieť vymazať položky alebo vytvoriť nový zoznam histórie.</span><span class="sxs-lookup"><span data-stu-id="b626d-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b626d-117">Ďalšie informácie: [Vymazanie histórie pracovného postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b626d-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b626d-118">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="b626d-118">Related topics</span></span>
<span data-ttu-id="b626d-119">Chcete vyskúšať službu Microsoft flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="b626d-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b626d-120">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="b626d-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b626d-121">SharePoint a flow</span><span class="sxs-lookup"><span data-stu-id="b626d-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


