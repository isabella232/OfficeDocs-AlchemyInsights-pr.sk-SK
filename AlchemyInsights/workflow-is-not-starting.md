---
title: Pracovný postup sa nes začatím
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403758"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="3a898-102">Pracovný postup sa nes začatím</span><span class="sxs-lookup"><span data-stu-id="3a898-102">Workflow is not starting</span></span>

- <span data-ttu-id="3a898-103">Pracovné postupy SharePointu 2010 a SharePointu 2013 sa nesajú.</span><span class="sxs-lookup"><span data-stu-id="3a898-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="3a898-104">Ak sa pracovný postup nes začatím nezačína, môže ísť o dočasný problém so službami, v rámci ktorého sa používateľom môžu vyskytnúť občasné oneskorenia s priebehom pracovného postupu.</span><span class="sxs-lookup"><span data-stu-id="3a898-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="3a898-105">Skontrolujte [tabuľu stavu služby a](https://admin.microsoft.com/AdminPortal/Home/servicehealth) zistite, či to bude mať vplyv na vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="3a898-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="3a898-106">Ak uplynulo viac než 24 hodín od toho, čo ste tento problém prvýkrát videli, prihláste sa do lístka technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="3a898-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3a898-107">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="3a898-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3a898-108">Dajte nám aspoň 24 hodín na dokončenie riešenia.</span><span class="sxs-lookup"><span data-stu-id="3a898-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="3a898-109">Pracovné postupy SharePointu 2010 sa oneskorili pri spustení.</span><span class="sxs-lookup"><span data-stu-id="3a898-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="3a898-110">Dochádza k tomu, ak sa pracovný postup spustí vo veľkých dávkach.</span><span class="sxs-lookup"><span data-stu-id="3a898-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="3a898-111">(napríklad, keď sa pridá niekoľko položiek naraz).</span><span class="sxs-lookup"><span data-stu-id="3a898-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="3a898-112">Pracovné postupy nie sú navrhnuté na spustenie v reálnom čase, preto je oneskorenie v štýle návrhu.</span><span class="sxs-lookup"><span data-stu-id="3a898-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="3a898-113">Ak je pracovný postup komplexný extensible Object Markup Language (XILE), kompilácia môže byť pomalá.</span><span class="sxs-lookup"><span data-stu-id="3a898-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="3a898-114">Pozrite [si tento](https://support.microsoft.com//kb/3043697) článok.</span><span class="sxs-lookup"><span data-stu-id="3a898-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="3a898-115">Pracovný postup by ste mali zjednodušiť alebo ho vylepšiť pomocou typu platformy Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="3a898-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="3a898-116">Ak sa história pracovného postupu príliš rozrástla, môžete položky vymazať alebo vytvoriť nový zoznam histórie.</span><span class="sxs-lookup"><span data-stu-id="3a898-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="3a898-117">Ďalšie informácie: [Vymazanie histórie pracovného postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="3a898-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="3a898-118">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="3a898-118">Related topics</span></span>
<span data-ttu-id="3a898-119">Chcete vyskúšať Microsoft Flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="3a898-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3a898-120">Vytvorenie toku</span><span class="sxs-lookup"><span data-stu-id="3a898-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3a898-121">SharePoint a Flow</span><span class="sxs-lookup"><span data-stu-id="3a898-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
