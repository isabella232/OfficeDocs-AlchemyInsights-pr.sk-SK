---
title: Read-Only na údržbu správy pri pokuse o použitie SharePoint alebo OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620738"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="b165a-102">Read-Only na údržbu správy pri pokuse o použitie SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="b165a-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="b165a-103">Používatelia môžu hlásenie **Read-Only pre údržbu** pri pokuse o použitie SharePoint alebo OneDrive pre jeden z týchto scenárov.</span><span class="sxs-lookup"><span data-stu-id="b165a-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="b165a-104">Plánované alebo aktívna údržba činnosť.</span><span class="sxs-lookup"><span data-stu-id="b165a-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="b165a-105">Skontrolovať ich prechodom do [Centra správ](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="b165a-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="b165a-106">Vysokou prioritou, aktívne servisné udalosti, ktorá môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="b165a-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="b165a-107">Kontrola každej návestí podpory incidentov, prechodom do [Služby zdravia](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b165a-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="b165a-108">Drobné automatické liečenie zotavenie scenár, ktorý mohol deje z dôvodu neočakávaných udalostí na serveroch, ktoré môže trvať menej ako 30 minút alebo tak.</span><span class="sxs-lookup"><span data-stu-id="b165a-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="b165a-109">Neexistujú žiadne Message Center alebo služby zdravia príspevky pre tieto menšie extrakcia, ale mali by ste byť späť do normálneho veľmi skoro.</span><span class="sxs-lookup"><span data-stu-id="b165a-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="b165a-110">Veľmi málo príležitostiach sme pozorovali, že jeden z troch scenárov uvedených vyššie boli príčinou, a služba bola obnovená, ale cache prehliadača užívateľov nemá očistili.</span><span class="sxs-lookup"><span data-stu-id="b165a-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="b165a-111">Prosím pokúsi zmazať cache prehliadača pred vyhľadania lokality.</span><span class="sxs-lookup"><span data-stu-id="b165a-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="b165a-112">V prehliadači Microsoft Edge, vyberte **nastavenia**a potom vyberte položku **súkromie a bezpečnosť**.</span><span class="sxs-lookup"><span data-stu-id="b165a-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="b165a-113">Podľa **jasných prehliadania**, vyberte položku **vybrať položky na vymazanie**.</span><span class="sxs-lookup"><span data-stu-id="b165a-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="b165a-114">Vyberte **súbory cookie a uložené údaje webových lokalít**a vyberte **Vymazať**.</span><span class="sxs-lookup"><span data-stu-id="b165a-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="b165a-115">Tieto kroky sa môžu líšiť, pri použití iných prehliadačov, ako Mozilla Firefox alebo Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="b165a-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="b165a-116">Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v nové okno v režime InPrivate.</span><span class="sxs-lookup"><span data-stu-id="b165a-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>