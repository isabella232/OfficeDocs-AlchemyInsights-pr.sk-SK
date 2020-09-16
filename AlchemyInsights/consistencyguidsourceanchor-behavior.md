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
# <a name="consistencyguid--sourceanchor-behavior"></a>Správanie ConsistencyGuid/sourceAnchor

Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie MSD – ConsistencyGuid ako atribút sourceAnchor. Pri použití tejto funkcie Služba Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie na:
  
- Použite MSD – ConsistencyGuid ako atribút sourceAnchor pre objekty používateľa. ObjectGUID sa používa pre iné typy objektov.
    
- Pre ľubovoľný objekt lokálneho objektu AD, ktorého atribút MSD – ConsistencyGuid nie je vyplnený, Azure AD Connect zapíše svoju objectGUID hodnotu späť do atribútu MSD – ConsistencyGuid v lokálnej službe Active Directory. Po vyplnení atribútu MSD – ConsistencyGuid Azure AD Connect potom exportuje objekt do služby Azure AD.
    
 **Poznámka:** Po importovaní lokálneho REKLAMNÉho objektu do služby Azure AD Connect (to znamená, že sa importuje do priestoru konektora reklamy a premieta sa do Metaverse), už nie je možné zmeniť jeho sourceAnchor hodnotu. Ak chcete zadať hodnotu sourceAnchor pre daný lokálny objekt AD, pred importovaním do služby Azure AD Connect nakonfigurujte atribút MSD – ConsistencyGuid. 
  
Ďalšie informácie o SourceAnchor a ConsistencyGuid nájdete v týchto témach: [návrh konceptov služby Azure AD Connect:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

