---
title: Prekročený denný limit e-mail. Pracovný postup pozastaví.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514485"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="7fbe1-103">Denné e-mail Limit prekročený.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="7fbe1-104">Pracovný postup pozastaví.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-104">Workflow is suspended.</span></span>

<span data-ttu-id="7fbe1-105">Táto chyba môže prijatá v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="7fbe1-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="7fbe1-106">Máte pracovného postupu SharePoint Online, používajúce SharePoint 2010 alebo SharePoint 2013 pracovného postupu typ platformy.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="7fbe1-107">Pracovný postup je nakonfigurovaný na odosielanie vlastné e-mailové správy vyše 200 používateľov, viac ako 10 000 príjemcov za deň, alebo viac ako 30 správ za minútu.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="7fbe1-108">Pri spustení toku činností, e-mailovú správu nie je odoslaná a môžete pozorovať nasledujúce správanie:</span><span class="sxs-lookup"><span data-stu-id="7fbe1-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="7fbe1-109">Pracovného postupu pomocou typ platformy SharePoint 2013, môžete prehľadávať na stránke **Stav toku činností** .</span><span class="sxs-lookup"><span data-stu-id="7fbe1-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="7fbe1-110">Na stránke stav toku činností **Vnútorný stav** je nastavený na **začal**a informácie balón zobrazuje **sa nedá Odoslať príjemcovi**.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="7fbe1-111">Ak chcete obísť tento problém, nakonfigurovať vaše workflow posielať e-maily bez prekročenia [Exchange Online odosielateľa limity](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="7fbe1-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="7fbe1-112">Napríklad pomocou pauza pracovného postupu, Odoslať e-mail do skupiny Office 365, distribučnú skupinu alebo skupiny zabezpečenia mail zapnuté alebo neodoslať menej než 200 príjemcom naraz.</span><span class="sxs-lookup"><span data-stu-id="7fbe1-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="7fbe1-113">Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="7fbe1-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="7fbe1-114">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="7fbe1-114">Related topics</span></span>
- [<span data-ttu-id="7fbe1-115">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="7fbe1-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7fbe1-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="7fbe1-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 