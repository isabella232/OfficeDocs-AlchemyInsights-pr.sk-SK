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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044355"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor behavior

Azure AD Pripojenie (verzia 1.1.524.0 a po) teraz uľahčuje používanie atribútu msDS-ConsistencyGuid ako atribút sourceAnchor. Pri používaní tejto funkcie Azure AD Pripojenie automaticky nakonfiguruje pravidlá synchronizácie na:
  
- Ako zdrojový atribútAnchor pre objekty používateľa použite príkaz msDS-ConsistencyGuid. ObjectGUID sa používa pre iné typy objektov.
    
- Pre každý objekt lokálneho používateľa služby AD, ktorého atribút msDS-ConsistencyGuid nie je vyplnený, Azure AD Pripojenie zapíše hodnotu objectGUID späť do atribútu msDS-ConsistencyGuid v lokálnej službe Active Directory. Po vyplnení atribútu msDS-ConsistencyGuid Azure AD Pripojenie objekt exportuje do služby Azure AD.
    
 **Poznámka:** Po importe lokálneho objektu AD do služby Azure AD Pripojenie (t. j. importované do priestoru konektora AD a projektované do metaverzovej funkcie) už nie je možné zmeniť jeho zdrojovú hodnotuAnchor. Ak chcete zadať hodnotu sourceAnchor pre daný lokálny objekt AD, nakonfigurujte atribút msDS-ConsistencyGuid ešte pred jeho importom do služby Azure AD Pripojenie. 
  
Ďalšie informácie o službe SourceAnchor a ConsistencyGuid nájdete v nasledujúcich informáciách: [Azure AD Pripojenie: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

