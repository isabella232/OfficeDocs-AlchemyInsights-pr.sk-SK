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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="47992-102">Otázky o používaní nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="47992-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="47992-103">Prevezmite nástroj na nasadenie balíka Office zo [strediska pre prevzatie softvéru spoločnosti Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="47992-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="47992-104">Po stiahnutí súboru, spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje nástroj na nasadenie balíka Office spustiteľný súbor (Setup. exe) a ukážkové konfiguračné súbory (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="47992-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="47992-105">**Vylúčiť alebo odstrániť Microsoft 365 aplikácie pre podnikové produkty z klientskych počítačov:**</span><span class="sxs-lookup"><span data-stu-id="47992-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="47992-106">Pri inštalácii aplikácií Microsoft 365 pre podniky môžete vylúčiť konkrétne produkty.</span><span class="sxs-lookup"><span data-stu-id="47992-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="47992-107">Vykonáte to tak, postupujte podľa pokynov pre inštaláciu balíka Office s ODT, ale zahrnúť ExcludeApp element v konfiguračnom súbore.</span><span class="sxs-lookup"><span data-stu-id="47992-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="47992-108">Napríklad, tento konfiguračný súbor nainštaluje všetky Microsoft 365 aplikácie pre podnikové produkty okrem vydavateľa:</span><span class="sxs-lookup"><span data-stu-id="47992-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="47992-109">Prehľad nástroja na nasadenie balíka Office</span><span class="sxs-lookup"><span data-stu-id="47992-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

