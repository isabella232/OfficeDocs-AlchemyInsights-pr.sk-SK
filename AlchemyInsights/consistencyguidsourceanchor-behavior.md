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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36517010"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor správanie

Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie msDS-ConsistencyGuid ako atribút sourceAnchor. Pri používaní tejto funkcie Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie na:
  
- Použite msDS-ConsistencyGuid ako atribút sourceAnchor pre objekty používateľa. ObjectGUID sa používa pre iné typy objektov.
    
- Pre ľubovoľný lokálny objekt používateľa AD, ktorého msDS-ConsistencyGuid atribút nie je vyplnený, Azure AD Connect píše jeho objectGUID hodnotu späť na msDS-ConsistencyGuid atribút lokálnej služby Active Directory. Po msDS-ConsistencyGuid atribút je vyplnený, Azure AD pripojiť potom exportuje objekt Azure AD.
    
 **Poznámka:** Keď je lokálny objekt AD importovaný do Azure AD Connect (čiže importovaný do priestoru pre reklamný konektor a plánovaný do Metaverse), už nie je možné zmeniť jeho hodnotu sourceAnchor. Ak chcete určiť hodnotu sourceAnchor pre daný lokálny objekt AD, nakonfigurujte jeho atribút msDS-ConsistencyGuid pred jeho importovaním do Azure AD Connect. 
  
Ďalšie informácie o SourceAnchor a ConsistencyGuid, označovať takto: [Azure AD Connect: Koncepty návrhov](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

