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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="c15aa-102">Otázky o používaní nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="c15aa-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c15aa-103">Prevezmite nástroj na nasadenie balíka Office zo [strediska pre prevzatie softvéru spoločnosti Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c15aa-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="c15aa-104">Po stiahnutí súboru, spustite samorozbaľovací spustiteľný súbor, ktorý obsahuje nástroj na nasadenie balíka Office spustiteľný súbor (Setup. exe) a ukážkové konfiguračné súbory (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="c15aa-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="c15aa-105">**Vylúčenie alebo odstránenie produktov balíka Office 365 ProPlus z klientskych počítačov:**</span><span class="sxs-lookup"><span data-stu-id="c15aa-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="c15aa-106">Pri inštalácii balíka Office 365 ProPlus môžete vylúčiť konkrétne produkty.</span><span class="sxs-lookup"><span data-stu-id="c15aa-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="c15aa-107">Vykonáte to tak, postupujte podľa pokynov pre inštaláciu balíka Office s ODT, ale zahrnúť ExcludeApp element v konfiguračnom súbore.</span><span class="sxs-lookup"><span data-stu-id="c15aa-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="c15aa-108">Napríklad, tento konfiguračný súbor nainštaluje všetky produkty balíka Office 365 ProPlus okrem vydavateľa:</span><span class="sxs-lookup"><span data-stu-id="c15aa-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="c15aa-109">Prehľad nástroja na nasadenie balíka Office</span><span class="sxs-lookup"><span data-stu-id="c15aa-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

