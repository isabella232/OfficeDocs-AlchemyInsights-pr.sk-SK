---
title: ConsistencyGuid / sourceAnchor správanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498533"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="e6290-102">ConsistencyGuid / sourceAnchor správanie</span><span class="sxs-lookup"><span data-stu-id="e6290-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="e6290-p101">Azure AD pripojiť (verzie 1.1.524.0 a po) teraz podporuje použitie BL-ConsistencyGuid ako atribút sourceAnchor. Pri použití tejto funkcie, Azure AD pripojiť automaticky konfiguruje pravidlá synchronizácie:</span><span class="sxs-lookup"><span data-stu-id="e6290-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="e6290-p102">Sko-ConsistencyGuid ako atribút sourceAnchor použiť pre používateľa objekty. ObjectGUID sa používa pre iné typy objektov.</span><span class="sxs-lookup"><span data-stu-id="e6290-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="e6290-p103">Pre ľubovoľnú danú lokálneho AD používateľa objekt ktorého MSD ConsistencyGuid atribút nie je vyplnený, Azure AD pripojenie píše svoju hodnotu objectGUID späť MSD ConsistencyGuid atribút v lokálnej služby Active Directory. Po MSD ConsistencyGuid atribút je vyplnený, Azure AD pripojiť potom exportuje objekt Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6290-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="e6290-p104">**Poznámka:** Raz lokálneho AD objektu dováža do Azure AD pripojiť (čiže dovezený do priestoru konektor AD a premieta do Metaverse), nemôžete zmeniť jeho sourceAnchor hodnotu anymore. Zadať sourceAnchor hodnotu pre dané lokálneho AD objekt, pred dováža do Azure AD pripojenie nakonfigurovať jeho MSD ConsistencyGuid atribút.</span><span class="sxs-lookup"><span data-stu-id="e6290-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="e6290-111">Pre viac informácií o SourceAnchor a ConsistencyGuid, označovať takto: [Azure AD pripojiť: vyklápateľným](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="e6290-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

