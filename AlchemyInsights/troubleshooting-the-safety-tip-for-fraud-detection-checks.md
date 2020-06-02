---
title: Riešenie problémov s bezpečnostným tipom na kontrolu podvodov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504998"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="0a7ad-102">Riešenie problémov s bezpečnostným tipom na kontrolu podvodov</span><span class="sxs-lookup"><span data-stu-id="0a7ad-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="0a7ad-103">Ak dostávate bezpečnostný tip s textom "Odosielateľ zlyhal pri kontrole podvodov a nemusí byť tým, kým sa zdá byť", potom sa odosielateľovi nepodarilo prejsť kontrolou overovania DKIM alebo SPF.</span><span class="sxs-lookup"><span data-stu-id="0a7ad-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="0a7ad-104">Najlepší spôsob, ako to vyriešiť, je pre odosielateľa, aby saautori sami.</span><span class="sxs-lookup"><span data-stu-id="0a7ad-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="0a7ad-105">Ak odosielateľ odosiela vo vašom mene, musíte ich autorizovať pridaním adresy IP odosielateľa do záznamu SPF.</span><span class="sxs-lookup"><span data-stu-id="0a7ad-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="0a7ad-106">Ďalšie informácie nájdete v časti [Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu podvodov.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)</span><span class="sxs-lookup"><span data-stu-id="0a7ad-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="0a7ad-107">Tu je niekoľko ďalších odkazov, ktoré môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="0a7ad-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="0a7ad-108">Ako spoločnosť Microsoft používa rámec politiky odosielateľa (SPF) na zabránenie falšovaniu</span><span class="sxs-lookup"><span data-stu-id="0a7ad-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="0a7ad-109">Nastavenie protokolu SPF na zabránenie falšovaniu</span><span class="sxs-lookup"><span data-stu-id="0a7ad-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
