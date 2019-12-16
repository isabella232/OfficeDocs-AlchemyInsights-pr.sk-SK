---
title: E-mail pracovného postupu sa neodosiela
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049388"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a6ea9-102">E-mail pracovného postupu sa neodosiela pre zoznam alebo knižnicu lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="a6ea9-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a6ea9-103">E-maily z pracovných postupov sa neodosielajú všetkým používateľom alebo len konkrétnym používateľom, alebo sa zobrazí chyba, **e-mailová správa sa nedá odoslať. Uistite sa, že e-mail má platného príjemcu**.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a6ea9-104">Skontrolujte, či používateľ existuje v skupine **všetky osoby** povolenia (zoznam informácií o používateľovi) pre túto kolekciu lokalít.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a6ea9-105">Ukážka priamej adresy URL:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="a6ea9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a6ea9-106">Ak používateľ neexistuje, uistite sa, že používateľ je prihlásený na stránku.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a6ea9-107">Ak ide o externého používateľa, uistite sa, že ich pozvánka bola prijatá.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a6ea9-108">Ak používateľ existuje v skupine povolenia, uistite sa, že e-mailová adresa je správna.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a6ea9-109">Ak e-mailová adresa používateľov nie je nastavená tu, potom vytvorte ukážkovú výstrahu pre daného používateľa, ktorá vynúti synchronizáciu daného používateľského konta z používateľských profilov lokality SharePoint do tejto kolekcie lokalít.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a6ea9-110">E-maily z pracovných postupov sa odosielajú správcom kolekcie lokalít, ale nie ostatným používateľom a zobrazí sa chyba **http zakázané <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a6ea9-111">Pozrite si [prístup odmietnutý pri odosielaní e-mailu do skupiny SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a6ea9-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a6ea9-112">Tiež overiť, že **obmedzený prístup používateľa povolenie Lockdown režime** kolekcie lokalít funkcia nie je aktívna.</span><span class="sxs-lookup"><span data-stu-id="a6ea9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a6ea9-113">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="a6ea9-113">Related topics</span></span>
<span data-ttu-id="a6ea9-114">Chcete vyskúšať službu Microsoft flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="a6ea9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a6ea9-115">Vytvoriť tok</span><span class="sxs-lookup"><span data-stu-id="a6ea9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a6ea9-116">SharePoint a flow</span><span class="sxs-lookup"><span data-stu-id="a6ea9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


