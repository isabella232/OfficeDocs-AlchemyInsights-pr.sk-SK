---
title: Prekročil sa limit denného e-mailu. Pracovný postup sa pozastavuje.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731578"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="55153-103">Prekročil sa limit denného e-mailu.</span><span class="sxs-lookup"><span data-stu-id="55153-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="55153-104">Pracovný postup sa pozastavuje.</span><span class="sxs-lookup"><span data-stu-id="55153-104">Workflow is suspended.</span></span>

<span data-ttu-id="55153-105">Táto chyba môže byť prijatá v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="55153-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="55153-106">Máte pracovný postup v SharePointe Online, ktorý používa typ platformy pracovného postupu SharePointu 2010 alebo SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="55153-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="55153-107">Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy viacerým používateľom vo 200, viac ako 10 000 príjemcov za deň alebo viac ako 30 správ za minútu.</span><span class="sxs-lookup"><span data-stu-id="55153-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="55153-108">Po spustení pracovného postupu sa e-mailová správa neodošle a všimnete si nasledovné správanie:</span><span class="sxs-lookup"><span data-stu-id="55153-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="55153-109">Ak používate pracovný postup s použitím typu platformy SharePoint 2013, prejdite na stránku **stavu pracovného postupu** .</span><span class="sxs-lookup"><span data-stu-id="55153-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="55153-110">Na stránke stav pracovného postupu je **vnútorný stav** nastavený na možnosť **Spustiť**a v bubline s informáciami sa **nedajú Odoslať príjemcovi**.</span><span class="sxs-lookup"><span data-stu-id="55153-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="55153-111">Ak chcete tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez prekročenia [limitov odosielateľov služby Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="55153-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="55153-112">Môžete napríklad použiť pauzu v pracovnom postupe, Odoslať e-mail do skupiny Microsoft 365, distribučnej skupiny alebo skupiny zabezpečenia s podporou e-mailu alebo Odoslať správu menej ako 200 príjemcom naraz.</span><span class="sxs-lookup"><span data-stu-id="55153-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="55153-113">Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="55153-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="55153-114">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="55153-114">Related topics</span></span>
- [<span data-ttu-id="55153-115">Vytvorenie toku</span><span class="sxs-lookup"><span data-stu-id="55153-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="55153-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="55153-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 