---
title: Prekročený denný limit e-mailov. Pracovný postup je pozastavený.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908719"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="0c832-103">Prekročený denný limit e-mailov.</span><span class="sxs-lookup"><span data-stu-id="0c832-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="0c832-104">Pracovný postup je pozastavený.</span><span class="sxs-lookup"><span data-stu-id="0c832-104">Workflow is suspended.</span></span>

<span data-ttu-id="0c832-105">Táto chyba môže byť prijatá v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="0c832-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="0c832-106">Máte pracovný postup SharePoint Online, ktorý používa typ platformy SharePoint 2010 alebo SharePoint 2013 pracovného postupu.</span><span class="sxs-lookup"><span data-stu-id="0c832-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="0c832-107">Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy na viac ako 200 používateľov naraz, viac ako 10 000 príjemcov za deň, alebo viac ako 30 správ za minútu.</span><span class="sxs-lookup"><span data-stu-id="0c832-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="0c832-108">Pri spustení pracovného postupu, e-mailová správa nie je odoslaná a zistíte nasledovné správanie:</span><span class="sxs-lookup"><span data-stu-id="0c832-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="0c832-109">Pre tok činností pomocou typu platformy SharePoint 2013, môžete prechádzať na stránke **stav pracovného postupu** .</span><span class="sxs-lookup"><span data-stu-id="0c832-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="0c832-110">Na stránke stav toku činností je **interný stav** nastavený na hodnotu **spustené**a informačný balón sa **nedá Odoslať príjemcovi**.</span><span class="sxs-lookup"><span data-stu-id="0c832-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="0c832-111">Tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez prekročenia [limitov odosielateľa Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="0c832-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="0c832-112">Napríklad, použite pauzu v toku činností, pošlite e-mail do skupiny Microsoft 365, distribučná skupina alebo poštové skupiny zabezpečenia povolené alebo Odoslať správu menej ako 200 príjemcov naraz.</span><span class="sxs-lookup"><span data-stu-id="0c832-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="0c832-113">Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="0c832-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="0c832-114">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="0c832-114">Related topics</span></span>
- [<span data-ttu-id="0c832-115">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="0c832-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0c832-116">SharePoint a flow</span><span class="sxs-lookup"><span data-stu-id="0c832-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 