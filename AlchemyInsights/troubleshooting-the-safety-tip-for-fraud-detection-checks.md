---
title: Riešenie problémov s bezpečnostnými tipmi na kontroly podvodov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834746"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c76db-102">Riešenie problémov s bezpečnostnými tipmi na kontroly podvodov</span><span class="sxs-lookup"><span data-stu-id="c76db-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c76db-103">Ak vám zobrazí bezpečnostný tip s o tom, že odosielateľ zlyhal z našich kontrol zisťovania podvodov a pravdepodobne nie tým, kým sa zdá byť," odosielateľ nedokázal odovzdať overovacie kontroly DKIM alebo SPF.</span><span class="sxs-lookup"><span data-stu-id="c76db-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c76db-104">Najlepším spôsobom riešenia tohto problému je, aby si odosielateľ povolil svoje povolenie.</span><span class="sxs-lookup"><span data-stu-id="c76db-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c76db-105">Ak odosielateľ odosiela správy vo vašom mene, je potrebné povoliť ho pridaním IP adresy odosielateľa do SPF záznamu.</span><span class="sxs-lookup"><span data-stu-id="c76db-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c76db-106">Ďalšie [informácie nájdete v téme Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) podvodov.</span><span class="sxs-lookup"><span data-stu-id="c76db-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c76db-107">Tu je niekoľko ďalších prepojení, ktoré vám môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="c76db-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c76db-108">Ako spoločnosť Microsoft používa SPF (Sender Policy Framework) na zabránenie predstierania predstierania odosielateľa</span><span class="sxs-lookup"><span data-stu-id="c76db-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c76db-109">Nastavenie SPF na zabránenie predstierania predstierania</span><span class="sxs-lookup"><span data-stu-id="c76db-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
