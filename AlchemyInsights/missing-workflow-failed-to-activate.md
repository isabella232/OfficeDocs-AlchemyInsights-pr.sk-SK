---
title: Chýbajúci pracovný postup sa nepodarilo aktivovať
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667101"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="b0dfe-102">Chýbajúci pracovný postup sa nepodarilo aktivovať</span><span class="sxs-lookup"><span data-stu-id="b0dfe-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="b0dfe-103">V kolekcii lokalít Microsoft SharePoint nie je možné do zoznamu alebo knižnice pridať globálne opätovne použiteľný pracovný postup (ako je napríklad "schválenie – SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="b0dfe-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b0dfe-104">Ak chcete tento problém vyriešiť, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="b0dfe-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b0dfe-105">Otvorte koreňovú webovú lokalitu kolekcie lokalít v SharePointe Designeri 2013.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b0dfe-106">V časti **objekty lokality**vyberte položku **pracovné postupy**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b0dfe-107">V **novej** časti pása s nástrojmi **pracovných postupov** vyberte položku **opätovne použiteľný pracovný postup**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b0dfe-108">Na formulári **vytvoriť opätovne použiteľný pracovný postup** zadajte názov \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="b0dfe-109">Pre **typ platformy**kliknite na položku **pracovný postup SharePointu 2010**a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b0dfe-110">V časti **Uložiť** na páse s nástrojmi **pracovný postup** vyberte položku **Publikovať**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b0dfe-111">V časti **Spravovať** na páse s nástrojmi **pracovný postup** vyberte položku **Publikovať na globálnej úrovni**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="b0dfe-112">V zobrazenom dialógovom okne potvrdenia vyberte položku **OK**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b0dfe-113">Vo webovom prehliadači vyhľadajte koreňovú webovú lokalitu kolekcie lokalít a potom kliknite na položku funkcie kolekcie lokalít v **časti Nastavenie lokality** \> **Site Collection Features**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="b0dfe-114">Potom prepnite funkciu **pracovné postupy** :</span><span class="sxs-lookup"><span data-stu-id="b0dfe-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b0dfe-115">· Ak je funkcia  *aktivovaná*  , kliknite na položku **deaktivovať** a potom kliknite na položku **aktivovať**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b0dfe-116">· Ak je funkcia  *deaktivovaná*  , kliknite na položku **aktivovať**.</span><span class="sxs-lookup"><span data-stu-id="b0dfe-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b0dfe-117">Ďalšie informácie nájdete v nasledujúcom [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b0dfe-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

