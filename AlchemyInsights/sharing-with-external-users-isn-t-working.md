---
title: Zdieľanie s externými používateľmi nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691590"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="870a6-102">Riešenie problémov s zdieľaním obsahu SharePointu s externými používateľmi</span><span class="sxs-lookup"><span data-stu-id="870a6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="870a6-103">Skontrolujte, či je pre vašu organizáciu zapnutá funkcia externého zdieľania:</span><span class="sxs-lookup"><span data-stu-id="870a6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="870a6-104">Prejdite na [ &amp; stránku doplnky služieb v centre spravovania služby Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na položku **lokality**.</span><span class="sxs-lookup"><span data-stu-id="870a6-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="870a6-105">Skontrolujte, či je nastavenie zapnuté.</span><span class="sxs-lookup"><span data-stu-id="870a6-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="870a6-106">Ak je vybratá možnosť len existujúci Externí používatelia, skontrolujte, či je externý používateľ uvedený v centre spravovania pre Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="870a6-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="870a6-107">Skontrolujte, či je externé zdieľanie pre lokalitu zapnuté.</span><span class="sxs-lookup"><span data-stu-id="870a6-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="870a6-108">Pre klasickú kolekciu lokalít:</span><span class="sxs-lookup"><span data-stu-id="870a6-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="870a6-109">V novom centre spravovania služby SharePoint kliknite na ľavej table na položku **lokality**.</span><span class="sxs-lookup"><span data-stu-id="870a6-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="870a6-110">Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.</span><span class="sxs-lookup"><span data-stu-id="870a6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="870a6-111">Pre tímovú lokalitu, ktorá patrí do skupiny Microsoft 365 alebo na komunikačnú lokalitu:</span><span class="sxs-lookup"><span data-stu-id="870a6-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="870a6-112">Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie celej organizácie, pokiaľ nastavenie pre celú organizáciu neumožňuje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="870a6-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="870a6-113">V tomto prípade lokality povoľujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlásia.</span><span class="sxs-lookup"><span data-stu-id="870a6-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="870a6-114">Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové centrum spravovania služby SharePoint alebo prostredie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="870a6-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="870a6-115">[Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="870a6-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="870a6-116">Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť reštriktívnejšie ako nastavenie celej organizácie, ale nie viac tolerantné ako nastavenie celej organizácie.</span><span class="sxs-lookup"><span data-stu-id="870a6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

