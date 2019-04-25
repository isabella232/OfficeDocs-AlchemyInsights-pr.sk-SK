---
title: ConsistencyGuid / sourceAnchor správanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408123"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="ac336-102">ConsistencyGuid / sourceAnchor správanie</span><span class="sxs-lookup"><span data-stu-id="ac336-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="ac336-103">Azure AD pripojiť (verzie 1.1.524.0 a po) teraz podporuje použitie BL-ConsistencyGuid ako atribút sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="ac336-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="ac336-104">Pri použití tejto funkcie, Azure AD pripojiť automaticky konfiguruje pravidlá synchronizácie:</span><span class="sxs-lookup"><span data-stu-id="ac336-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="ac336-105">Sko-ConsistencyGuid ako atribút sourceAnchor použiť pre používateľa objekty.</span><span class="sxs-lookup"><span data-stu-id="ac336-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="ac336-106">ObjectGUID sa používa pre iné typy objektov.</span><span class="sxs-lookup"><span data-stu-id="ac336-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="ac336-107">Pre ľubovoľnú danú lokálneho AD používateľa objekt ktorého MSD ConsistencyGuid atribút nie je vyplnený, Azure AD pripojenie píše svoju hodnotu objectGUID späť MSD ConsistencyGuid atribút v lokálnej služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ac336-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="ac336-108">Po MSD ConsistencyGuid atribút je vyplnený, Azure AD pripojiť potom exportuje objekt Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac336-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="ac336-109">**Poznámka:** Raz lokálneho AD objektu dováža do Azure AD pripojiť (čiže dovezený do priestoru konektor AD a premieta do Metaverse), nemôžete zmeniť jeho sourceAnchor hodnotu anymore.</span><span class="sxs-lookup"><span data-stu-id="ac336-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="ac336-110">Zadať sourceAnchor hodnotu pre dané lokálneho AD objekt, pred dováža do Azure AD pripojenie nakonfigurovať jeho MSD ConsistencyGuid atribút.</span><span class="sxs-lookup"><span data-stu-id="ac336-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="ac336-111">Pre viac informácií o SourceAnchor a ConsistencyGuid, označovať takto: [Azure AD pripojiť: vyklápateľným](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="ac336-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

