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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916539"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Najčastejším dôvodom pre AttributeValueMustBeUnique chyba je dvoch objektov s rôznymi SourceAnchor (immutableId) majú rovnakú hodnotu pre ProxyAddresses alebo UserPrincipalName atribúty. Opraviť AttributeValueMustBeUnique chyba:
  
1. Identifikáciu duplicitných proxyAddresses, userPrincipalName alebo iné hodnoty atribútu, ktorý spôsobuje chybu. Tiež určiť, ktoré objekty dvoch (alebo viacerých) sú zapojené do konfliktu. Správy generované Azure AD pripojiť zdravie pre synchronizáciu môže pomôcť identifikovať dva objekty.
    
2. Určiť predmet, ktorý by mal mať duplicitné hodnoty aj naďalej a predmet, ktorý by nemal.
    
3. Odstráňte duplicitné hodnoty objektu, že by nemali mať túto hodnotu. Všimnite si, že by mal urobiť zmeny v adresári kde sa objekt pochádza z. V niektorých prípadoch budete musieť odstrániť objekty v konflikte.
    
4. Ak ste vykonali zmeny v objekte na reklamu, nech Azure AD pripojiť synchronizovať zmeny pre chyby opravené.
    

