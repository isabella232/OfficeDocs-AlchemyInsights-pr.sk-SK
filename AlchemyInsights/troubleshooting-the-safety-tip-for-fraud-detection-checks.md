---
title: Troubleshooting bezpečnosť tip pre odhaľovanie podvodov kontroly
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658130"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="f78bd-102">Troubleshooting bezpečnosť tip pre odhaľovanie podvodov kontroly</span><span class="sxs-lookup"><span data-stu-id="f78bd-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="f78bd-p101">Ak ste získali bezpečnostné tip, že hovorí "odosielateľ nepodarilo našej kontroly detekcie podvodov a ktorí sa zdajú byť možno" potom odosielateľa sa nepodarilo prejsť SPF alebo DKIM overovacie kontroly. Najlepší spôsob, ako vyriešiť tento problém je pre odosielateľa povoliť sami. Ak odosielateľ posiela vo vašom mene, musíte povoliť pridaním IP adresa odosielateľa na záznam SPF.</span><span class="sxs-lookup"><span data-stu-id="f78bd-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="f78bd-106">Pozri [Riešenie problémov červená (podozrivé) bezpečnostné tip pre odhaľovanie podvodov kontroly](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="f78bd-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="f78bd-107">Tu sú niektoré ďalšie odkazy, ktoré môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="f78bd-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="f78bd-108">Ako Office 365 používa odosielateľa politický rámec (SPF) zabraňuje predstieraniu iného odosielateľa</span><span class="sxs-lookup"><span data-stu-id="f78bd-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="f78bd-109">Nastaviť SPF v Office 365 na zabránenie spoofing</span><span class="sxs-lookup"><span data-stu-id="f78bd-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

