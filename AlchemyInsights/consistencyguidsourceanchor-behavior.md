---
title: ConsistencyGuid/sourceAnchor správanie
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36517010"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="5b514-102">ConsistencyGuid/sourceAnchor správanie</span><span class="sxs-lookup"><span data-stu-id="5b514-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="5b514-103">Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie msDS-ConsistencyGuid ako atribút sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="5b514-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="5b514-104">Pri používaní tejto funkcie Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie na:</span><span class="sxs-lookup"><span data-stu-id="5b514-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="5b514-105">Použite msDS-ConsistencyGuid ako atribút sourceAnchor pre objekty používateľa.</span><span class="sxs-lookup"><span data-stu-id="5b514-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="5b514-106">ObjectGUID sa používa pre iné typy objektov.</span><span class="sxs-lookup"><span data-stu-id="5b514-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="5b514-107">Pre ľubovoľný lokálny objekt používateľa AD, ktorého msDS-ConsistencyGuid atribút nie je vyplnený, Azure AD Connect píše jeho objectGUID hodnotu späť na msDS-ConsistencyGuid atribút lokálnej služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b514-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="5b514-108">Po msDS-ConsistencyGuid atribút je vyplnený, Azure AD pripojiť potom exportuje objekt Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5b514-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="5b514-109">**Poznámka:** Keď je lokálny objekt AD importovaný do Azure AD Connect (čiže importovaný do priestoru pre reklamný konektor a plánovaný do Metaverse), už nie je možné zmeniť jeho hodnotu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="5b514-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="5b514-110">Ak chcete určiť hodnotu sourceAnchor pre daný lokálny objekt AD, nakonfigurujte jeho atribút msDS-ConsistencyGuid pred jeho importovaním do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5b514-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="5b514-111">Ďalšie informácie o SourceAnchor a ConsistencyGuid, označovať takto: [Azure AD Connect: Koncepty návrhov](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="5b514-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

