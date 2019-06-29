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
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353264"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="89b60-102">Troubleshooting bezpečnosť tip pre odhaľovanie podvodov kontroly</span><span class="sxs-lookup"><span data-stu-id="89b60-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="89b60-103">Ak ste získali bezpečnostné tip, že hovorí "odosielateľ nepodarilo našej kontroly detekcie podvodov a ktorí sa zdajú byť možno" potom odosielateľa sa nepodarilo prejsť SPF alebo DKIM overovacie kontroly.</span><span class="sxs-lookup"><span data-stu-id="89b60-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="89b60-104">Najlepší spôsob, ako vyriešiť tento problém je pre odosielateľa povoliť sami.</span><span class="sxs-lookup"><span data-stu-id="89b60-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="89b60-105">Ak odosielateľ posiela vo vašom mene, musíte povoliť pridaním IP adresa odosielateľa na záznam SPF.</span><span class="sxs-lookup"><span data-stu-id="89b60-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="89b60-106">Pozri [Riešenie problémov červená (podozrivé) bezpečnostné tip pre odhaľovanie podvodov kontroly](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="89b60-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="89b60-107">Tu sú niektoré ďalšie odkazy, ktoré môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="89b60-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="89b60-108">Ako Office 365 používa odosielateľa politický rámec (SPF) zabraňuje predstieraniu iného odosielateľa</span><span class="sxs-lookup"><span data-stu-id="89b60-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="89b60-109">Nastaviť SPF v Office 365 na zabránenie spoofing</span><span class="sxs-lookup"><span data-stu-id="89b60-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
