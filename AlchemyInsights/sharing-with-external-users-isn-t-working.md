---
title: Zdieľania s externými používateľmi nepracuje
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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753441"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="6b5d9-102">Riešenie problémov zdieľania obsahu SharePoint s externými používateľmi</span><span class="sxs-lookup"><span data-stu-id="6b5d9-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="6b5d9-103">Uistite sa, že externé zdieľanie je zapnutý pre vašu organizáciu:</span><span class="sxs-lookup"><span data-stu-id="6b5d9-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="6b5d9-104">Prejsť na [služby &amp; pridať-ins stránku Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a kliknite na tlačidlo **lokality**.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="6b5d9-105">Skontrolujte nastavenie je nastavená na "Zap."</span><span class="sxs-lookup"><span data-stu-id="6b5d9-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="6b5d9-106">Ak je vybratá "Len existujúce externých používateľov", uistite sa, že externý používateľ je uvedená Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="6b5d9-107">Uistite sa, že externé zdieľanie je zapnutá pre lokalitu.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="6b5d9-108">Klasické kolekcie:</span><span class="sxs-lookup"><span data-stu-id="6b5d9-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="6b5d9-109">Klasické SharePoint admin Center, na ľavej table kliknite na položku **kolekcie lokalít**.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="6b5d9-110">Vyberte lokality, ani lokality a na páse s nástrojmi, kliknite na položku **Zdieľanie**.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="6b5d9-111">Pre tímovú lokalitu, ktorá patrí do skupiny Office 365 alebo lokalitu komunikácie:</span><span class="sxs-lookup"><span data-stu-id="6b5d9-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="6b5d9-112">Tieto nové typy lokalít majú rovnaké zdieľanie nastavenie ako nastavenie pre celú organizáciu, ak nastavenie celej organizácii umožňuje zdieľanie súborov pomocou odkazov, ktoré nevyžadujú prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="6b5d9-113">V tomto prípade stránky umožňujú zdieľanie nových a existujúcich externých používateľov, ktorí prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="6b5d9-114">Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové SharePoint admin center (Ukážka) alebo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="6b5d9-115">[Zistite viac](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="6b5d9-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="6b5d9-116">Externé nastavenie zdieľania na ľubovoľnej lokalite môže byť reštriktívnejšie než nastavenia pre celú organizáciu, ale nie zhovievavejšie ako nastavenie celej organizácie.</span><span class="sxs-lookup"><span data-stu-id="6b5d9-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

