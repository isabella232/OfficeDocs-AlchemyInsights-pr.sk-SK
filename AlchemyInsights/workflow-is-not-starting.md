---
title: Tok činností sa nespustí
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270795"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="0c71e-102">Tok činností sa nespustí</span><span class="sxs-lookup"><span data-stu-id="0c71e-102">Workflow is not starting</span></span>

- <span data-ttu-id="0c71e-103">Pracovné postupy služby SharePoint 2010 a SharePoint 2013 sa nespustí.</span><span class="sxs-lookup"><span data-stu-id="0c71e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="0c71e-104">Ak váš pracovný postup sa nedá spustiť, tam môže byť problém pri dočasnej služby tam, kde používatelia môžu vyskytnúť občasné meškanie s workflow pokrok.</span><span class="sxs-lookup"><span data-stu-id="0c71e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="0c71e-105">Kontrola [Tabuľa stav služby](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) zistiť, ak vaša organizácia je ovplyvnené.</span><span class="sxs-lookup"><span data-stu-id="0c71e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="0c71e-106">Ak uplynulo viac ako 24 hodín od najprv ste videli tento problém, prihláste sa prosím na podporu lístok.</span><span class="sxs-lookup"><span data-stu-id="0c71e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="0c71e-107">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="0c71e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0c71e-108">Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.</span><span class="sxs-lookup"><span data-stu-id="0c71e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="0c71e-109">Pracovné postupy služby SharePoint 2010 odložené na Štart.</span><span class="sxs-lookup"><span data-stu-id="0c71e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="0c71e-110">V takom prípade pracovný postup sa spustí vo veľkých sériách.</span><span class="sxs-lookup"><span data-stu-id="0c71e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="0c71e-111">(napríklad keď niekoľko položky sú pridané naraz).</span><span class="sxs-lookup"><span data-stu-id="0c71e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="0c71e-112">Toky činností nie sú určené na spustiť v reálnom čase, takže oneskorenie je-design správanie.</span><span class="sxs-lookup"><span data-stu-id="0c71e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="0c71e-113">Ak tok činností je zložité Extensible Object Markup jazyk (XMol) od, kompilácia môže byť pomalé.</span><span class="sxs-lookup"><span data-stu-id="0c71e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="0c71e-114">Pozrite [Tento](https://support.microsoft.com/en-us/kb/3043697) článok.</span><span class="sxs-lookup"><span data-stu-id="0c71e-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="0c71e-115">By mala zjednodušiť pracovného postupu alebo redesign pomocou typ platformy Microsoft SharePoint 2013 pracovného postupu.</span><span class="sxs-lookup"><span data-stu-id="0c71e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="0c71e-116">Ak históriu toku činností Veľká, chcete položky vymazať alebo vytvoriť nový zoznam histórie.</span><span class="sxs-lookup"><span data-stu-id="0c71e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="0c71e-117">Viac informácií: [Vymazanie histórie toku činností](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="0c71e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="0c71e-118">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="0c71e-118">Related topics</span></span>
<span data-ttu-id="0c71e-119">Chceš skúsiť Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="0c71e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0c71e-120">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="0c71e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0c71e-121">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="0c71e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


