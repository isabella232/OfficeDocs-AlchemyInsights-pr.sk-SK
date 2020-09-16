---
title: Správanie ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756298"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="877ac-102">Správanie ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="877ac-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="877ac-103">Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie MSD – ConsistencyGuid ako atribút sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="877ac-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="877ac-104">Pri použití tejto funkcie Služba Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie na:</span><span class="sxs-lookup"><span data-stu-id="877ac-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="877ac-105">Použite MSD – ConsistencyGuid ako atribút sourceAnchor pre objekty používateľa.</span><span class="sxs-lookup"><span data-stu-id="877ac-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="877ac-106">ObjectGUID sa používa pre iné typy objektov.</span><span class="sxs-lookup"><span data-stu-id="877ac-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="877ac-107">Pre ľubovoľný objekt lokálneho objektu AD, ktorého atribút MSD – ConsistencyGuid nie je vyplnený, Azure AD Connect zapíše svoju objectGUID hodnotu späť do atribútu MSD – ConsistencyGuid v lokálnej službe Active Directory.</span><span class="sxs-lookup"><span data-stu-id="877ac-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="877ac-108">Po vyplnení atribútu MSD – ConsistencyGuid Azure AD Connect potom exportuje objekt do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="877ac-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="877ac-109">**Poznámka:** Po importovaní lokálneho REKLAMNÉho objektu do služby Azure AD Connect (to znamená, že sa importuje do priestoru konektora reklamy a premieta sa do Metaverse), už nie je možné zmeniť jeho sourceAnchor hodnotu.</span><span class="sxs-lookup"><span data-stu-id="877ac-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="877ac-110">Ak chcete zadať hodnotu sourceAnchor pre daný lokálny objekt AD, pred importovaním do služby Azure AD Connect nakonfigurujte atribút MSD – ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="877ac-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="877ac-111">Ďalšie informácie o SourceAnchor a ConsistencyGuid nájdete v týchto témach: [návrh konceptov služby Azure AD Connect:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="877ac-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

