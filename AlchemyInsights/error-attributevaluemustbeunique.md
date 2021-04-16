---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813775"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AtribútValueMustBeUnique

Najčastejším dôvodom chyby AtribútValueMustBeUnique sú dva objekty s odlišným atribútom SourceAnchor (immutableId), ktoré majú rovnakú hodnotu pre atribúty ProxyAddresses a/alebo UserPrincipalName. Oprava chyby AtribútValueMustBeUnique:
  
1. Identifikujte duplicitné proxyAddresses, userPrincipalName alebo inú hodnotu atribútu, ktorá spôsobuje chybu. Určite, ktoré dva (alebo viac) objektov sa v konflikte zúčastňujú. Zostava vygenerovaná službou Azure AD Connect Health na synchronizáciu vám môže pomôcť identifikovať dva objekty.
    
2. Identifikujte, ktorý objekt by mal mať naďalej duplicitnú hodnotu a ktorý objekt by nemal mať.
    
3. Odstráňte z objektu duplicitnú hodnotu, ktorá NEMÁ túto hodnotu mať. Mali by ste vykonať zmenu v adresári, z ktorého je objekt zdroj. V niektorých prípadoch budete musieť odstrániť jeden z objektov, ktoré sú v konflikte.
    
4. Ak ste vykonali zmenu v lokálnej službe AD, povoľte službe Azure AD Connect synchronizovať zmenu, aby sa problém vyriešil.
    

