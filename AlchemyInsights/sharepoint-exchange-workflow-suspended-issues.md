---
title: Začíname so službou SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700722"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="3a4a3-102">Pracovné postupy v SharePointe</span><span class="sxs-lookup"><span data-stu-id="3a4a3-102">Workflows in SharePoint</span></span>

<span data-ttu-id="3a4a3-103">Ak pracovné postupy SharePointu neodosielajú e-maily, vaša organizácia sa mohla stretnúť s obmedzeniami odosielateľa v službe Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3a4a3-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="3a4a3-104">Chybové hlásenie "pracovný postup je pozastavené" sa môže vyskytnúť, ak máte jednu z nasledujúcich položiek:</span><span class="sxs-lookup"><span data-stu-id="3a4a3-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="3a4a3-105">Máte pracovný postup v SharePointe Online, ktorý používa typ platformy pracovného postupu SharePointu 2010 alebo SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="3a4a3-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="3a4a3-106">Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy viacerým používateľom vo 200, viac ako 10 000 príjemcov za deň alebo viac ako 30 správ za minútu.</span><span class="sxs-lookup"><span data-stu-id="3a4a3-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="3a4a3-107">Keď spustíte pracovný postup, e-mailová správa sa neodošle a zistíte, že sa zobrazí chybové hlásenie, interný stav je nastavený na možnosť pozastavené alebo nie je možné Odoslať príjemcovi.</span><span class="sxs-lookup"><span data-stu-id="3a4a3-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="3a4a3-108">Ďalšie informácie nájdete v nasledujúcom [článku](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="3a4a3-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

