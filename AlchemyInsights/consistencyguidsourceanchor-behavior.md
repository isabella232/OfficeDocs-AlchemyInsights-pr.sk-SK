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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517010"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor správanie

Azure AD pripojiť (verzie 1.1.524.0 a po) teraz podporuje použitie BL-ConsistencyGuid ako atribút sourceAnchor. Pri použití tejto funkcie, Azure AD pripojiť automaticky konfiguruje pravidlá synchronizácie:
  
- Sko-ConsistencyGuid ako atribút sourceAnchor použiť pre používateľa objekty. ObjectGUID sa používa pre iné typy objektov.
    
- Pre ľubovoľnú danú lokálneho AD používateľa objekt ktorého MSD ConsistencyGuid atribút nie je vyplnený, Azure AD pripojenie píše svoju hodnotu objectGUID späť MSD ConsistencyGuid atribút v lokálnej služby Active Directory. Po MSD ConsistencyGuid atribút je vyplnený, Azure AD pripojiť potom exportuje objekt Azure AD.
    
 **Poznámka:** Raz lokálneho AD objektu dováža do Azure AD pripojiť (čiže dovezený do priestoru konektor AD a premieta do Metaverse), nemôžete zmeniť jeho sourceAnchor hodnotu anymore. Zadať sourceAnchor hodnotu pre dané lokálneho AD objekt, pred dováža do Azure AD pripojenie nakonfigurovať jeho MSD ConsistencyGuid atribút. 
  
Pre viac informácií o SourceAnchor a ConsistencyGuid, označovať takto: [Azure AD pripojiť: vyklápateľným](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

