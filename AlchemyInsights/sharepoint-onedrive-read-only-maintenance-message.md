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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840530"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="2fac8-102">Read-Only na údržbu správy pri pokuse o použitie SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="2fac8-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="2fac8-103">Používatelia môžu hlásenie **Iba na čítanie pre údržbu** pri pokuse o použitie SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2fac8-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="2fac8-104">Ak áno, skontrolujte, či je aktívna údržba vyskytujúce sa na nájomcu prechodom do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="2fac8-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="2fac8-105">Tiež, uistite sa, že kontrola tabuľa [Stav služby](https://portal.office.com/adminportal/home#/servicehealth) zistiť akékoľvek upozornenia/incidentov, ktoré sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="2fac8-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="2fac8-106">Ak ani centra správ alebo služby zdravia dashboard uviedli niečo o bežná údržba pre nájomcu, môže to byť prehliadač caching problém.</span><span class="sxs-lookup"><span data-stu-id="2fac8-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="2fac8-107">Prosím pokúsi zmazať cache prehliadača pred vyhľadania lokality.</span><span class="sxs-lookup"><span data-stu-id="2fac8-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="2fac8-108">V prehliadači Microsoft Edge, vyberte **nastavenia**a potom vyberte položku **súkromie a bezpečnosť**.</span><span class="sxs-lookup"><span data-stu-id="2fac8-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="2fac8-109">Podľa **jasných prehliadania**, vyberte položku **vybrať položky na vymazanie**.</span><span class="sxs-lookup"><span data-stu-id="2fac8-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="2fac8-110">Vyberte **súbory cookie a uložené údaje webových lokalít**a vyberte **Vymazať**.</span><span class="sxs-lookup"><span data-stu-id="2fac8-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="2fac8-111">Tieto kroky sa môžu líšiť, pri použití iných prehliadačov, ako Mozilla Firefox alebo Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="2fac8-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="2fac8-112">Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v nové okno v režime InPrivate.</span><span class="sxs-lookup"><span data-stu-id="2fac8-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>