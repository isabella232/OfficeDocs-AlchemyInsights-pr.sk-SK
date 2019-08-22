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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530904"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="6470f-102">Workflow email nie odošle do zoznamu SharePoint alebo knižnice</span><span class="sxs-lookup"><span data-stu-id="6470f-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="6470f-103">E-mail od toky činností nie sú odoslané do všetkých používateľov alebo iba určitým používateľom alebo vidíte chybu **e-mailovú správu nemožno odoslať. Uistite sa, e-mailu má platný príjemcu**.</span><span class="sxs-lookup"><span data-stu-id="6470f-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="6470f-104">Skontrolujte, či používateľ existovať v skupine povolenia **Všetkým ľuďom** (zoznam informácií o používateľoch) pre túto kolekciu lokalít.</span><span class="sxs-lookup"><span data-stu-id="6470f-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="6470f-105">Ochutnajte priame URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="6470f-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="6470f-106">Ak používateľ neexistuje, uistite sa, že používateľ je podpísaná do stránky.</span><span class="sxs-lookup"><span data-stu-id="6470f-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="6470f-107">Ak je externého používateľa, uistite sa, že ich pozvania.</span><span class="sxs-lookup"><span data-stu-id="6470f-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="6470f-108">Ak používateľ neexistuje v skupine povolenia, uistite sa, že e-mailová adresa je správna.</span><span class="sxs-lookup"><span data-stu-id="6470f-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="6470f-109">Ak užívatelia e-mailová adresa je tu, potom vytvoriť ukážku upozornenia pre daného používateľa, ktorá núti synchronizácie používateľského konta z používateľské profily SharePoint do kolekcie lokality.</span><span class="sxs-lookup"><span data-stu-id="6470f-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="6470f-110">E-mail od pracovných postupov sa odosielajú správcovia kolekcie lokalít, ale nie iných používateľov a zobraziť chyba **HTTP zakázané na <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="6470f-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="6470f-111">Vidieť [Prístup odmietnutý keď pošlete e-mail do skupiny SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="6470f-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="6470f-112">Tiež skontrolujte, že funkcie kolekcie lokality **obmedzeným prístupom používateľ povolenie uzamknutie režime** nie je aktívny.</span><span class="sxs-lookup"><span data-stu-id="6470f-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="6470f-113">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="6470f-113">Related topics</span></span>
<span data-ttu-id="6470f-114">Chceš skúsiť Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6470f-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6470f-115">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="6470f-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6470f-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="6470f-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


