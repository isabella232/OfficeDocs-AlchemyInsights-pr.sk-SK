---
title: Otázky o používaní nástroja na nasadenie balíka Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010773"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky o používaní nástroja na nasadenie balíka Office (ODT)

Prevezmite nástroj na nasadenie balíka Office zo [strediska pre prevzatie softvéru spoločnosti Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po stiahnutí súboru, spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje nástroj na nasadenie balíka Office spustiteľný súbor (Setup. exe) a ukážkové konfiguračné súbory (Configuration. xml).
  
 **Vylúčiť alebo odstrániť Microsoft 365 aplikácie pre podnikové produkty z klientskych počítačov:**
  
Pri inštalácii aplikácií Microsoft 365 pre podniky môžete vylúčiť konkrétne produkty. Vykonáte to tak, postupujte podľa pokynov pre inštaláciu balíka Office s ODT, ale zahrnúť ExcludeApp element v konfiguračnom súbore. Napríklad, tento konfiguračný súbor nainštaluje všetky Microsoft 365 aplikácie pre podnikové produkty okrem vydavateľa:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

