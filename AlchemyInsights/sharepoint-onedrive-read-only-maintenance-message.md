---
title: Iba na čítanie správy o údržbe pri pokuse o používanie SharePointu alebo OneDrivu
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
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670847"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="bd148-102">Iba na čítanie správy o údržbe pri pokuse o používanie SharePointu alebo OneDrivu</span><span class="sxs-lookup"><span data-stu-id="bd148-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="bd148-103">Pri pokuse o používanie SharePointu alebo OneDrivu pre niektorý z nasledujúcich scenárov môžu používatelia dostávať správu o **údržbe iba na čítanie** .</span><span class="sxs-lookup"><span data-stu-id="bd148-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="bd148-104">Plánovaná alebo aktívna aktivita údržby.</span><span class="sxs-lookup"><span data-stu-id="bd148-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="bd148-105">Vyhľadajte ich tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="bd148-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="bd148-106">Aktívny incident služby s vysokou prioritou, ktorý sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="bd148-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="bd148-107">Vyhľadajte všetky upozornenia alebo incidenty navigáciou na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="bd148-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="bd148-108">Malý scenár obnovenia automatického hojenia, ktorý by sa mohol stať v dôsledku neočakávaných udalostí na serveroch, ktoré môžu trvať menej ako 30 minút alebo tak.</span><span class="sxs-lookup"><span data-stu-id="bd148-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="bd148-109">Nie sú k dispozícii žiadne centrá správ ani príspevky týkajúce sa zdravotníckych služieb pre tieto drobné zotavuje, ale mali by ste sa vrátiť k normálu veľmi skoro.</span><span class="sxs-lookup"><span data-stu-id="bd148-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="bd148-110">Pri veľmi málo príležitostiach sme zistili, že jedným z týchto troch scenárov boli príčiny a služba bola obnovená, ale vyrovnávacia pamäť prehliadača používateľov nebola vymazaná.</span><span class="sxs-lookup"><span data-stu-id="bd148-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="bd148-111">Skôr než prejdete na lokalitu, skúste vymazať vyrovnávaciu pamäť prehliadača.</span><span class="sxs-lookup"><span data-stu-id="bd148-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="bd148-112">V prehliadači Microsoft Edge vyberte položku **Nastavenie**a potom vyberte položku **Ochrana osobných údajov a zabezpečenie**.</span><span class="sxs-lookup"><span data-stu-id="bd148-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="bd148-113">V časti **Vymazanie prehľadávania**vyberte položku **vybrať položky, ktoré chcete vymazať**.</span><span class="sxs-lookup"><span data-stu-id="bd148-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="bd148-114">Vyberte položku **súbory cookie a uložené údaje webovej lokality**a vyberte položku **Vymazať**.</span><span class="sxs-lookup"><span data-stu-id="bd148-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="bd148-115">Tieto kroky sa môžu líšiť pri používaní iných prehliadačov, ako je napríklad Mozilla Firefox alebo Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="bd148-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="bd148-116">Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v novom okne v režime InPrivate.</span><span class="sxs-lookup"><span data-stu-id="bd148-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>