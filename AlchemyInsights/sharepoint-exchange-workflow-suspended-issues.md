---
title: Začíname s SharePointom online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051656"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="0e03e-102">Toky činností v službe SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e03e-102">Workflows in SharePoint</span></span>

<span data-ttu-id="0e03e-103">Ak pracovné postupy služby SharePoint neodosielajú e-maily, vaša organizácia pravdepodobne narazila na limity odosielateľa Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0e03e-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="0e03e-104">"Workflow je pozastavená" chybové hlásenie sa môže vyskytnúť, ak máte jednu z nasledujúcich položiek:</span><span class="sxs-lookup"><span data-stu-id="0e03e-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="0e03e-105">Máte pracovný postup SharePoint Online, ktorý používa typ platformy SharePoint 2010 alebo SharePoint 2013 pracovného postupu.</span><span class="sxs-lookup"><span data-stu-id="0e03e-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="0e03e-106">Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy na viac ako 200 používateľov naraz, viac ako 10 000 príjemcov za deň, alebo viac ako 30 správ za minútu.</span><span class="sxs-lookup"><span data-stu-id="0e03e-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="0e03e-107">Pri spustení pracovného postupu, e-mailová správa nie je odoslaná, a zistíte, že chybové hlásenie, interný stav je nastavený na pozastavené alebo nie je možné Odoslať príjemcovi sa zobrazí.</span><span class="sxs-lookup"><span data-stu-id="0e03e-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="0e03e-108">Ďalšie informácie nájdete v nasledujúcom [článku](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="0e03e-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

