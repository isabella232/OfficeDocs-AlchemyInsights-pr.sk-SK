---
title: Otázky o používaní nástroja na nasadenie balíka Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086171"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky o používaní nástroja na nasadenie balíka Office (ODT)

Stiahnite si nástroj na nasadenie balíka Office z [Centra sťahovania](https://go.microsoft.com/fwlink/p/?LinkID=626065)softvéru.
  
Po stiahnutí súboru spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje spustiteľný súbor nástroja na nasadenie balíka Office (setupodt.exe) a ukážkový konfiguračný súbor (configuration.xml).
  
 **Vylúčenie alebo odstránenie aplikácií Microsoft 365 pre podnikové produkty z klientskych počítačov:**
  
Pri inštalácii aplikácií Microsoft 365 pre podniky môžete vylúčiť konkrétne produkty. Ak to chcete urobiť, postupujte podľa krokov na inštaláciu balíka Office s formátom ODT, ale do konfiguračného súboru zadajte prvok ExcludeApp. Tento konfiguračný súbor napríklad nainštaluje všetky aplikácie Microsoft 365 pre podnikové produkty okrem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

