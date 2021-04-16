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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="75849-102">Otázky o používaní nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="75849-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="75849-103">Stiahnite si Nástroj na nasadenie balíka Office z [Centra sťahovania softvéru spoločnosti Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="75849-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="75849-104">Po stiahnutí súboru spustite samoobslužný spustiteľný súbor, ktorý obsahuje spustiteľný nástroj na nasadenie balíka Office (setup.exe) a vzorový konfiguračný súbor (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="75849-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="75849-105">**Vylúčenie alebo odstránenie aplikácií Microsoft 365 pre podnikové produkty z klientskych počítačov:**</span><span class="sxs-lookup"><span data-stu-id="75849-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="75849-106">Pri inštalácii aplikácií Microsoft 365 pre veľké podniky môžete vylúčiť konkrétne produkty.</span><span class="sxs-lookup"><span data-stu-id="75849-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="75849-107">Postupujte podľa krokov na inštaláciu balíka Office s ODT, ale do konfiguračného súboru zahrňte prvok ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="75849-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="75849-108">Týmto konfiguračným súborom sa napríklad nainštalujú všetky aplikácie Microsoft 365 pre podnikové produkty okrem Publishera:</span><span class="sxs-lookup"><span data-stu-id="75849-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="75849-109">Prehľad nástroja na nasadenie balíka Office</span><span class="sxs-lookup"><span data-stu-id="75849-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

