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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207700"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="fbca6-102">Riešenie problémov zdieľania obsahu SharePoint s externými používateľmi</span><span class="sxs-lookup"><span data-stu-id="fbca6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="fbca6-103">Uistite sa, že externé zdieľanie je zapnutý pre vašu organizáciu:</span><span class="sxs-lookup"><span data-stu-id="fbca6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="fbca6-104">Prejsť na [služby &amp; pridať-ins stránku Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a kliknite na tlačidlo **lokality**.</span><span class="sxs-lookup"><span data-stu-id="fbca6-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="fbca6-p101">Skontrolujte nastavenie je nastavená na "Zap." Ak je vybratá "Len existujúce externých používateľov", uistite sa, že externý používateľ je uvedená Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="fbca6-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="fbca6-p102">Uistite sa, že externé zdieľanie je zapnutá pre lokalitu. Klasické kolekcie:</span><span class="sxs-lookup"><span data-stu-id="fbca6-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="fbca6-109">Klasické SharePoint admin Center, na ľavej table kliknite na položku **kolekcie lokalít**.</span><span class="sxs-lookup"><span data-stu-id="fbca6-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="fbca6-110">Vyberte lokality, ani lokality a na páse s nástrojmi, kliknite na položku **Zdieľanie**.</span><span class="sxs-lookup"><span data-stu-id="fbca6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="fbca6-111">Pre tímovú lokalitu, ktorá patrí do skupiny Office 365 alebo lokalitu komunikácie:</span><span class="sxs-lookup"><span data-stu-id="fbca6-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="fbca6-p103">Tieto nové typy lokalít majú rovnaké zdieľanie nastavenie ako nastavenie pre celú organizáciu, ak nastavenie celej organizácii umožňuje zdieľanie súborov pomocou odkazov, ktoré nevyžadujú prihlásenie. V tomto prípade stránky umožňujú zdieľanie nových a existujúcich externých používateľov, ktorí prihlásenie. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové SharePoint admin center (Ukážka) alebo PowerShell. [Zistite viac](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="fbca6-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="fbca6-116">Externé nastavenie zdieľania na ľubovoľnej lokalite môže byť reštriktívnejšie než nastavenia pre celú organizáciu, ale nie zhovievavejšie ako nastavenie celej organizácie.</span><span class="sxs-lookup"><span data-stu-id="fbca6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

