---
title: Otázky o používaní nástroja na nasadenie balíka Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553555"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky o používaní nástroja na nasadenie balíka Office (ODT)

Prevezmite nástroj na nasadenie balíka Office zo [strediska pre prevzatie softvéru spoločnosti Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po stiahnutí súboru, spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje nástroj na nasadenie balíka Office spustiteľný súbor (Setup. exe) a ukážkové konfiguračné súbory (Configuration. xml).
  
 **Vylúčenie alebo odstránenie produktov balíka Office 365 ProPlus z klientskych počítačov:**
  
Pri inštalácii balíka Office 365 ProPlus môžete vylúčiť konkrétne produkty. Vykonáte to tak, postupujte podľa pokynov pre inštaláciu balíka Office s ODT, ale zahrnúť ExcludeApp element v konfiguračnom súbore. Napríklad, tento konfiguračný súbor nainštaluje všetky produkty balíka Office 365 ProPlus okrem vydavateľa:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

