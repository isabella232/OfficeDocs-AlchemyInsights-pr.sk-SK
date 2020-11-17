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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="db765-102">Otázky o používaní nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="db765-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="db765-103">Stiahnite si nástroj na nasadenie balíka Office z [Centra sťahovania](https://go.microsoft.com/fwlink/p/?LinkID=626065)softvéru.</span><span class="sxs-lookup"><span data-stu-id="db765-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="db765-104">Po stiahnutí súboru spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje spustiteľný súbor nástroja na nasadenie balíka Office (setupodt.exe) a ukážkový konfiguračný súbor (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="db765-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="db765-105">**Vylúčenie alebo odstránenie aplikácií Microsoft 365 pre podnikové produkty z klientskych počítačov:**</span><span class="sxs-lookup"><span data-stu-id="db765-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="db765-106">Pri inštalácii aplikácií Microsoft 365 pre podniky môžete vylúčiť konkrétne produkty.</span><span class="sxs-lookup"><span data-stu-id="db765-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="db765-107">Ak to chcete urobiť, postupujte podľa krokov na inštaláciu balíka Office s formátom ODT, ale do konfiguračného súboru zadajte prvok ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="db765-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="db765-108">Tento konfiguračný súbor napríklad nainštaluje všetky aplikácie Microsoft 365 pre podnikové produkty okrem programu Publisher:</span><span class="sxs-lookup"><span data-stu-id="db765-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="db765-109">Prehľad nástroja na nasadenie balíka Office</span><span class="sxs-lookup"><span data-stu-id="db765-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

