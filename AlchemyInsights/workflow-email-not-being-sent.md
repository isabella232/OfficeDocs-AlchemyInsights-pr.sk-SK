---
title: Odoslanie e-mailu v pracovnom postupe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749004"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="36d17-102">E-mail pracovného postupu sa neodosiela v zozname alebo knižnici SharePointu</span><span class="sxs-lookup"><span data-stu-id="36d17-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="36d17-103">E-maily z pracovných postupov sa neodosielajú všetkým používateľom ani iba konkrétnym používateľom alebo sa zobrazí chyba, **že sa e-mailová správa nedá odoslať. Skontrolujte, či má e-mail platný príjemca**.</span><span class="sxs-lookup"><span data-stu-id="36d17-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="36d17-104">Skontrolujte, či sa používateľ nachádza v skupine **všetci používatelia** (zoznam informácií o používateľoch) pre danú kolekciu lokalít.</span><span class="sxs-lookup"><span data-stu-id="36d17-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="36d17-105">Ukážka priameho URL adresy: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="36d17-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="36d17-106">Ak používateľ neexistuje, skontrolujte, či je používateľ prihlásený na stránku.</span><span class="sxs-lookup"><span data-stu-id="36d17-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="36d17-107">Ak ide o externého používateľa, skontrolujte, či bola pozvánka prijatá.</span><span class="sxs-lookup"><span data-stu-id="36d17-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="36d17-108">Ak používateľ v skupine povolenia existuje, skontrolujte, či je e-mailová adresa správna.</span><span class="sxs-lookup"><span data-stu-id="36d17-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="36d17-109">Ak tu nie je nastavená e-mailová adresa používateľov, potom vytvorte vzorové Upozornenie pre daného používateľa, ktoré vynúti synchronizáciu daného používateľského konta z používateľských profilov SharePointu do tejto kolekcie lokalít.</span><span class="sxs-lookup"><span data-stu-id="36d17-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="36d17-110">E-maily z pracovných postupov sa odosielajú správcom kolekcie lokalít, ale nie ostatným používateľom a zobrazí sa chyba **http Forbidden to <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="36d17-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="36d17-111">Pozrite si tému [prístup odmietnutý pri odoslaní e-mailu do skupiny SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="36d17-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="36d17-112">Skontrolujte tiež, či nie je aktívna funkcia **obmedzeného prístupu používateľa na uzamknutie režimu uzamknutia** lokality.</span><span class="sxs-lookup"><span data-stu-id="36d17-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="36d17-113">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="36d17-113">Related topics</span></span>
<span data-ttu-id="36d17-114">Chcete vyskúšať Microsoft flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="36d17-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="36d17-115">Vytvorenie toku</span><span class="sxs-lookup"><span data-stu-id="36d17-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="36d17-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="36d17-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


