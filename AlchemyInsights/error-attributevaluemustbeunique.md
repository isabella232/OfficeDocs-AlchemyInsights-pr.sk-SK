---
title: Chyba AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36527056"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Najčastejším dôvodom pre Attributhodnoemustbeunique chyba je dva objekty s rôznymi SourceAnchor (immutableId) majú rovnakú hodnotu pre ProxyAddresses a/alebo UserPrincipalName atribúty. Oprava AttributeValueMustBeUnique chyba:
  
1. Identifikujte duplicitné proxyAddresses, userPrincipalName alebo inú hodnotu atribútu, ktorá spôsobuje chybu. Tiež určiť, ktoré dva (alebo viac) objekty sú zapojené do konfliktu. Zostava vygenerovaná Azure AD Connect Health for Sync vám môže pomôcť identifikovať dva objekty.
    
2. Určiť, ktorý objekt by mal mať aj naďalej duplicitné hodnoty a ktoré objekt by nemal.
    
3. Odstrániť duplicitné hodnoty z objektu, ktorý by nemal mať túto hodnotu. Všimnite si, že by ste mali vykonať zmeny v adresári, kde objekt pochádza z. V niektorých prípadoch možno budete musieť odstrániť jeden z objektov v konflikte.
    
4. Ak ste vykonali zmeny v lokálnom AD, nech Azure AD pripojiť synchronizáciu zmeny chyby sa dostať fixné.
    

