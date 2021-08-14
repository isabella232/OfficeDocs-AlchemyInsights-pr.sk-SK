---
title: Otázky týkajúce sa používania nástroja Office na nasadenie (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959698"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky týkajúce sa používania nástroja Office na nasadenie (ODT)

Stiahnite si nástroj Office na nasadenie z Centra [sťahovania softvéru spoločnosti Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Po stiahnutí súboru spustite samoobslužný spustiteľný súbor, ktorý obsahuje spustiteľný nástroj na nasadenie balíka Office (setup.exe) a vzorový konfiguračný súbor (configuration.xml).
  
 **Vylúčenie alebo odstránenie produktov Aplikácie Microsoft 365 pre veľké organizácie z klientskych počítačov:**
  
Pri inštalácii Aplikácie Microsoft 365 pre veľké organizácie môžete vylúčiť konkrétne produkty. Ak to chcete urobiť, postupujte podľa krokov na Office s ODT, ale do konfiguračného súboru zahrňte prvok ExcludeApp. Tento konfiguračný súbor napríklad nainštaluje všetky produkty Aplikácie Microsoft 365 pre veľké organizácie okrem Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prehľad nástroja Office na nasadenie](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

