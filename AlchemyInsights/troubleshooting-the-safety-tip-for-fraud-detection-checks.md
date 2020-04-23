---
title: Riešenie problémov s bezpečnostným hrotom pre kontroly detekcie podvodov
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
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759527"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="4c9b0-102">Riešenie problémov s bezpečnostným hrotom pre kontroly detekcie podvodov</span><span class="sxs-lookup"><span data-stu-id="4c9b0-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="4c9b0-103">Ak ste získali bezpečnostný tip, ktorý hovorí, že "odosielateľ zlyhal naše kontroly podvodov detekcie a nemusí byť, kto sa zdajú byť", potom odosielateľ zlyhal odovzdať buď DKIM alebo SPF overovanie kontroly.</span><span class="sxs-lookup"><span data-stu-id="4c9b0-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="4c9b0-104">Najlepšia metóda na vyriešenie tohto problému je pre odosielateľa, ktorý sa má autorizovať.</span><span class="sxs-lookup"><span data-stu-id="4c9b0-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="4c9b0-105">Ak odosielateľ odosiela váš účet, musíte ich autorizovať pridaním adresy IP odosielateľa do záznamu SPF.</span><span class="sxs-lookup"><span data-stu-id="4c9b0-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="4c9b0-106">Ďalšie informácie nájdete [v téme Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu podvodov](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="4c9b0-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="4c9b0-107">Tu je niekoľko ďalších prepojení, ktoré môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="4c9b0-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="4c9b0-108">Ako Microsoft používa odosielateľa politiky rámec (SPF) zabrániť falšovanie</span><span class="sxs-lookup"><span data-stu-id="4c9b0-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="4c9b0-109">Nastavenie SPF na zabránenie falošnej spoofing</span><span class="sxs-lookup"><span data-stu-id="4c9b0-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
