---
title: ConsistencyGuid /sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817007"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="77a91-102">ConsistencyGuid /sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="77a91-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="77a91-103">Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie atribútu msDS-ConsistencyGuid ako atribút sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="77a91-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="77a91-104">Pri používaní tejto funkcie Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie tak, aby:</span><span class="sxs-lookup"><span data-stu-id="77a91-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="77a91-105">Ako zdrojový atribútAnchor pre objekty používateľa použite príkaz msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="77a91-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="77a91-106">ObjectGUID sa používa pre iné typy objektov.</span><span class="sxs-lookup"><span data-stu-id="77a91-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="77a91-107">Pre každý objekt lokálneho používateľa služby AD, ktorého atribút msDS-ConsistencyGuid nie je vyplnený, Azure AD Connect zapíše hodnotu objectGUID späť do atribútu msDS-ConsistencyGuid v lokálnej službe Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77a91-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="77a91-108">Po vyplnení atribútu msDS-ConsistencyGuid Azure AD Connect exportuje objekt do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="77a91-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="77a91-109">**Poznámka:** Po importe lokálneho objektu AD do služby Azure AD Connect (t. j. importovaní do priestoru konektora AD a projektovaní do metaverznej služby) už nie je možné zmeniť jeho zdrojovú hodnotuAnchor.</span><span class="sxs-lookup"><span data-stu-id="77a91-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="77a91-110">Ak chcete zadať hodnotu sourceAnchor pre daný lokálny objekt AD, nakonfigurujte jeho atribút msDS-ConsistencyGuid pred jeho importom do služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="77a91-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="77a91-111">Ďalšie informácie o službe SourceAnchor a ConsistencyGuid nájdete v nasledujúcich informáciách: [Azure AD Connect: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="77a91-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

