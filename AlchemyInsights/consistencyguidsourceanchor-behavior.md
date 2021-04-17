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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor behavior

Azure AD Connect (verzia 1.1.524.0 a po) teraz uľahčuje používanie atribútu msDS-ConsistencyGuid ako atribút sourceAnchor. Pri používaní tejto funkcie Azure AD Connect automaticky nakonfiguruje pravidlá synchronizácie tak, aby:
  
- Ako zdrojový atribútAnchor pre objekty používateľa použite príkaz msDS-ConsistencyGuid. ObjectGUID sa používa pre iné typy objektov.
    
- Pre každý objekt lokálneho používateľa služby AD, ktorého atribút msDS-ConsistencyGuid nie je vyplnený, Azure AD Connect zapíše hodnotu objectGUID späť do atribútu msDS-ConsistencyGuid v lokálnej službe Active Directory. Po vyplnení atribútu msDS-ConsistencyGuid Azure AD Connect exportuje objekt do služby Azure AD.
    
 **Poznámka:** Po importe lokálneho objektu AD do služby Azure AD Connect (t. j. importovaní do priestoru konektora AD a projektovaní do metaverznej služby) už nie je možné zmeniť jeho zdrojovú hodnotuAnchor. Ak chcete zadať hodnotu sourceAnchor pre daný lokálny objekt AD, nakonfigurujte jeho atribút msDS-ConsistencyGuid pred jeho importom do služby Azure AD Connect. 
  
Ďalšie informácie o službe SourceAnchor a ConsistencyGuid nájdete v nasledujúcich informáciách: [Azure AD Connect: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

