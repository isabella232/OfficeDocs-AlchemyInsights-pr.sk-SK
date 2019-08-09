---
title: Workflow e-mail sa odosiela nie
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
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270687"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="48ada-102">Workflow e-mail sa odosiela nie</span><span class="sxs-lookup"><span data-stu-id="48ada-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="48ada-103">E-mail od toky činností nie sú odoslané do všetkých používateľov alebo iba určitým používateľom alebo vidíte chybu **e-mailovú správu nemožno odoslať. Uistite sa, e-mailu má platný príjemcu**.</span><span class="sxs-lookup"><span data-stu-id="48ada-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="48ada-104">Skontrolujte, či používateľ existovať v skupine povolenia **Všetkým ľuďom** (zoznam informácií o používateľoch) pre túto kolekciu lokalít.</span><span class="sxs-lookup"><span data-stu-id="48ada-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="48ada-105">Ochutnajte priame URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="48ada-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="48ada-106">Ak používateľ neexistuje, uistite sa, že používateľ je podpísaná do stránky.</span><span class="sxs-lookup"><span data-stu-id="48ada-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="48ada-107">Ak je externého používateľa, uistite sa, že ich pozvania.</span><span class="sxs-lookup"><span data-stu-id="48ada-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="48ada-108">Ak používateľ neexistuje v skupine povolenia, uistite sa, že e-mailová adresa je správna.</span><span class="sxs-lookup"><span data-stu-id="48ada-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="48ada-109">Ak užívatelia e-mailová adresa je tu, potom vytvoriť ukážku upozornenia pre daného používateľa, ktorá núti synchronizácie používateľského konta z používateľské profily SharePoint do kolekcie lokality.</span><span class="sxs-lookup"><span data-stu-id="48ada-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="48ada-110">E-mail od pracovných postupov sa odosielajú správcovia kolekcie lokalít, ale nie iných používateľov a zobraziť chyba \*\*HTTP zakázané na <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="48ada-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="48ada-111">Vidieť [Prístup odmietnutý pri e-mail do skupiny](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="48ada-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="48ada-112">Tiež skontrolujte, že funkcie kolekcie lokality **obmedzeným prístupom používateľ povolenie uzamknutie režime** nie je aktívny.</span><span class="sxs-lookup"><span data-stu-id="48ada-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="48ada-113">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="48ada-113">Related topics</span></span>
<span data-ttu-id="48ada-114">Chceš skúsiť Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="48ada-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="48ada-115">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="48ada-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="48ada-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="48ada-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


