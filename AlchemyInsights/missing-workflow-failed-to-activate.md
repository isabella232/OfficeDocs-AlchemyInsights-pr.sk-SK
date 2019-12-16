---
title: Chýbajúci pracovný postup sa nepodarilo aktivovať
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052628"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="f67a9-102">Chýbajúci pracovný postup sa nepodarilo aktivovať</span><span class="sxs-lookup"><span data-stu-id="f67a9-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="f67a9-103">V kolekcii lokality Microsoft SharePoint, nemôžete pridať globálne opakovane pracovného postupu (napríklad "schválenie-SharePoint 2010") do zoznamu alebo knižnice.</span><span class="sxs-lookup"><span data-stu-id="f67a9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f67a9-104">Ak chcete vyriešiť tento problém, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="f67a9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f67a9-105">Otvorte koreňovú webovú lokalitu kolekcie lokalít v programe SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f67a9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f67a9-106">V časti **objekty lokality**vyberte položku **toky činností**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f67a9-107">V **novej** časti pása s nástrojmi **pracovné postupy** , vyberte **opakovane použiteľný pracovný postup**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f67a9-108">Vo formulári **vytvoriť opakovane použiteľný pracovný postup** zadajte názov \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="f67a9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f67a9-109">Pre **platformu typ**, kliknite na tlačidlo **SharePoint 2010 workflow**, a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f67a9-110">V časti **Uložiť** na páse s nástrojmi **pracovného postupu** vyberte **Publikovať**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f67a9-111">V časti **Správa** pása s nástrojmi **pracovného postupu** vyberte položku **Publikovať globálne**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f67a9-112">V zobrazenom dialógovom okne s potvrdením vyberte položku **OK**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f67a9-113">Vo webovom prehľadávači vyhľadajte koreňovú webovú lokalitu kolekcie lokalít a **potom prístup k** \> **funkciám kolekcie**lokality.</span><span class="sxs-lookup"><span data-stu-id="f67a9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f67a9-114">Potom prepnite funkciu **toky činností** :</span><span class="sxs-lookup"><span data-stu-id="f67a9-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f67a9-115">· Ak je funkcia *aktivovaná* , kliknite na tlačidlo **deaktivovať** a potom kliknite na tlačidlo **aktivovať**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f67a9-116">· Ak je funkcia *deaktivovaná* , kliknite na tlačidlo **aktivovať**.</span><span class="sxs-lookup"><span data-stu-id="f67a9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f67a9-117">Ďalšie informácie nájdete v nasledujúcom [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f67a9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

