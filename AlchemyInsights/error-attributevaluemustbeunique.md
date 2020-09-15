---
title: Chyba AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709166"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Najčastejšou príčinou chyby AttributeValueMustBeUnique sú dva objekty s rôznymi SourceAnchor (immutableId) majú rovnakú hodnotu pre ProxyAddresses a/alebo UserPrincipalName atribúty. Oprava chyby AttributeValueMustBeUnique:
  
1. Identifikujte duplikované proxyAddresses, userPrincipalName alebo inú hodnotu atribútu, ktorá spôsobuje chybu. Tiež Identifikujte, ktoré dva (alebo viac) objekty sa v konflikte zúčastňujú. Zostava vytvorená službou Azure AD Connect Health for Sync vám pomôže identifikovať dva objekty.
    
2. Identifikujte objekt, ktorý by mal mať aj naďalej duplicitnú hodnotu a objekt, ktorý by nemal.
    
3. Odstráňte duplicitnú hodnotu z objektu, ktorý by nemal mať túto hodnotu. Všimnite si, že by ste mali vykonať zmeny v adresári, v ktorom je objekt z zdroja. V niektorých prípadoch možno budete musieť odstrániť niektorý z objektov v konflikte.
    
4. Ak ste vykonali zmeny v lokálnej REKLAMe, nechajte službu Azure AD Connect synchronizácie zmeniť, aby sa vyskytla chyba.
    

