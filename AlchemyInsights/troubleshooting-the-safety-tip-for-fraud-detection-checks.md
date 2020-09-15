---
title: Riešenie problémov s bezpečnostnou špičkou pri kontrole podvodov
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658425"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="979de-102">Riešenie problémov s bezpečnostnou špičkou pri kontrole podvodov</span><span class="sxs-lookup"><span data-stu-id="979de-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="979de-103">Ak sa vám zobrazuje bezpečnostný tip s upozornením, že odosielateľ zlyhal pri kontrole odhaľovania podvodov a nemusí byť tým, komu sa zdá, že odosielateľ zlyhal pri overovaní overovacích kontrol.</span><span class="sxs-lookup"><span data-stu-id="979de-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="979de-104">Najvhodnejší spôsob riešenia tohto problému je umožniť odosielateľovi autorizovať seba.</span><span class="sxs-lookup"><span data-stu-id="979de-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="979de-105">Ak odosielateľ odosiela vo vašom mene, musíte ich povoliť pridaním IP adresy odosielateľa do SPF záznamu.</span><span class="sxs-lookup"><span data-stu-id="979de-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="979de-106">Ďalšie informácie nájdete [v téme Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu podvodov](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="979de-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="979de-107">Tu je niekoľko ďalších prepojení, ktoré vám môžu pomôcť:</span><span class="sxs-lookup"><span data-stu-id="979de-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="979de-108">Ako spoločnosť Microsoft používa na prevenciu spoofing rámec politiky odosielateľa (SPF)</span><span class="sxs-lookup"><span data-stu-id="979de-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="979de-109">Nastavenie SPF na prevenciu spoofing</span><span class="sxs-lookup"><span data-stu-id="979de-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
