---
title: Iba na čítanie pre správu údržby pri pokuse o použitie SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051296"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="1bc6d-102">Iba na čítanie pre správu údržby pri pokuse o použitie SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="1bc6d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="1bc6d-103">Používatelia môžu zobraziť **iba na čítanie pre údržbu** správy pri pokuse o použitie SharePoint alebo OneDrive pre jeden z nasledujúcich scenárov.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="1bc6d-104">Plánovanej alebo aktívnej činnosti údržby.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="1bc6d-105">Vyhľadajte ich tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="1bc6d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="1bc6d-106">Vysoká priorita, aktívny servisný incident, ktorý môže byť vyskytujúci sa.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="1bc6d-107">Vyhľadajte všetky upozornenia/incidenty tým, že prejdete na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1bc6d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="1bc6d-108">Menšie auto-liečenie zotavenie scenár, ktorý by mohol byť deje v dôsledku neočakávaných udalostí na serveroch, ktoré by mohli trvať menej ako 30 min alebo tak.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="1bc6d-109">Neexistujú žiadne správy centra alebo služby zdravia miest pre tieto drobné vymáhanie, ale mali by ste byť späť do normálu veľmi skoro.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="1bc6d-110">Na veľmi málo príležitostiach sme pozorovali, že jeden z troch scenárov uvedených vyššie boli príčinou, a služba bola obnovená, ale užívatelia prehliadač cache nebol vymazaný.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="1bc6d-111">Pred navigáciou na lokalitu sa pokúste vymazať vyrovnávaciu pamäť prehľadávača.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="1bc6d-112">V prehľadávači Microsoft Edge vyberte položku **Nastavenie**a potom vyberte položku **Ochrana osobných údajov a zabezpečenie**.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="1bc6d-113">V časti **Vymazanie prehľadávania**vyberte položku **vybrať, čo sa má vymazať**.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="1bc6d-114">Vyberte položku **súbory cookie a uložené údaje webových stránok**a vyberte položku **Vymazať**.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="1bc6d-115">Tieto kroky sa môžu líšiť pri používaní iných prehliadačov, ako je Mozilla Firefox alebo Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="1bc6d-116">Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v novom okne v režime InPrivate.</span><span class="sxs-lookup"><span data-stu-id="1bc6d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>