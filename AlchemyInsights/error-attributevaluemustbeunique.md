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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002135"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AtribútValueMustBeUnique

Najčastejším dôvodom chyby AtribútValueMustBeUnique sú dva objekty s odlišným atribútom SourceAnchor (immutableId), ktoré majú rovnakú hodnotu pre atribúty ProxyAddresses a/alebo UserPrincipalName. Oprava chyby AtribútValueMustBeUnique:
  
1. Identifikujte duplicitné proxyAddresses, userPrincipalName alebo inú hodnotu atribútu, ktorá spôsobuje chybu. Určite, ktoré dva (alebo viac) objektov sa v konflikte zúčastňujú. Zostava vygenerovaná službou Azure AD Pripojenie Health for sync vám môže pomôcť identifikovať dva objekty.
    
2. Identifikujte, ktorý objekt by mal mať naďalej duplicitnú hodnotu a ktorý objekt by nemal mať.
    
3. Odstráňte z objektu duplicitnú hodnotu, ktorá NEMÁ túto hodnotu mať. Mali by ste vykonať zmenu v adresári, z ktorého je objekt zdroj. V niektorých prípadoch budete musieť odstrániť jeden z objektov, ktoré sú v konflikte.
    
4. Ak ste vykonali zmenu v lokálnej službe AD, nechajte službu Azure AD Pripojenie synchronizáciu zmeny, aby sa chyba opravili.
    

