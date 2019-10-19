---
title: Zdieľanie s externými používateľmi nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502246"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="37759-102">Riešenie problémov s zdieľaním obsahu služby SharePoint s externými používateľmi</span><span class="sxs-lookup"><span data-stu-id="37759-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="37759-103">Presvedčte sa, či je pre vašu organizáciu zapnuté externé zdieľanie:</span><span class="sxs-lookup"><span data-stu-id="37759-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="37759-104">Prejdite na [stránku služby &amp; doplnky Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na tlačidlo **lokality**.</span><span class="sxs-lookup"><span data-stu-id="37759-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="37759-105">Presvedčte sa, či je nastavenie zapnuté "zapnuté".</span><span class="sxs-lookup"><span data-stu-id="37759-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="37759-106">Ak je vybratá možnosť "iba existujúcich externých používateľov", uistite sa, že externý používateľ je uvedený v Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="37759-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="37759-107">Skontrolujte, či je pre lokalitu zapnuté externé zdieľanie.</span><span class="sxs-lookup"><span data-stu-id="37759-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="37759-108">Pre klasickú kolekciu lokalít:</span><span class="sxs-lookup"><span data-stu-id="37759-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="37759-109">V novom SharePoint admin Center, na ľavej table kliknite na položku **lokality**.</span><span class="sxs-lookup"><span data-stu-id="37759-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="37759-110">Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.</span><span class="sxs-lookup"><span data-stu-id="37759-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="37759-111">Pre tímovú lokalitu, ktorá patrí do skupiny Office 365 alebo na komunikačnú lokalitu:</span><span class="sxs-lookup"><span data-stu-id="37759-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="37759-112">Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie pre celú organizáciu, pokiaľ nastavenie pre celú organizáciu umožňuje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="37759-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="37759-113">V tomto prípade lokality umožňujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlasujú.</span><span class="sxs-lookup"><span data-stu-id="37759-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="37759-114">Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové centrum spravovania služby SharePoint alebo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="37759-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="37759-115">Ďalšie [informácie](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="37759-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="37759-116">Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť obmedzujúcejšie ako nastavenie pre celú organizáciu, ale nie viac tolerantnejšie ako nastavenie celej organizácie.</span><span class="sxs-lookup"><span data-stu-id="37759-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

