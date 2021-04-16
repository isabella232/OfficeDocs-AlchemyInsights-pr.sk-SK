---
title: Otázky o používaní nástroja na nasadenie balíka Office (ODT)
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
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790347"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky o používaní nástroja na nasadenie balíka Office (ODT)

Stiahnite si Nástroj na nasadenie balíka Office z [Centra sťahovania softvéru spoločnosti Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Po stiahnutí súboru spustite samoobslužný spustiteľný súbor, ktorý obsahuje spustiteľný nástroj na nasadenie balíka Office (setup.exe) a vzorový konfiguračný súbor (configuration.xml).
  
 **Vylúčenie alebo odstránenie aplikácií Microsoft 365 pre podnikové produkty z klientskych počítačov:**
  
Pri inštalácii aplikácií Microsoft 365 pre veľké podniky môžete vylúčiť konkrétne produkty. Postupujte podľa krokov na inštaláciu balíka Office s ODT, ale do konfiguračného súboru zahrňte prvok ExcludeApp. Týmto konfiguračným súborom sa napríklad nainštalujú všetky aplikácie Microsoft 365 pre podnikové produkty okrem Publishera:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

