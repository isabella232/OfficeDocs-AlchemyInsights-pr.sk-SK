---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821426"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="406e6-102">Odstránenie problémov s doručovaním e-mailov s kódom chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="406e6-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="406e6-103">Overte SPF DNS záznam svojej domény na verejne dostupnej kontrole SPF alebo DNS záznamu na webe.</span><span class="sxs-lookup"><span data-stu-id="406e6-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="406e6-104">Overte, či spoločnosť Microsoft nei už odchádzajúca správa nebola identifikovaná ako nevyžiadaná pošta a smerovala cez Fond doručovania [s vysokým rizikom.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="406e6-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="406e6-105">Správy z fondu doručovania s vysokým rizikom neprejdú kontrolami SPF, a preto ich cieľová e-mailová organizácia nebude prijímať.</span><span class="sxs-lookup"><span data-stu-id="406e6-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="406e6-106">Ak problém pretrváva, možno bude potrebné obrátiť sa na správcu poštového hostiteľa, ktorému sa pokúšate odoslať e-mail.</span><span class="sxs-lookup"><span data-stu-id="406e6-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="406e6-107">Všimnite si podrobnú externú chybu, ktorá je k dispozícii v odrazovej správe.</span><span class="sxs-lookup"><span data-stu-id="406e6-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="406e6-108">Podpora spoločnosti Microsoft vám možno nebude vedieť pomôcť ďalej.</span><span class="sxs-lookup"><span data-stu-id="406e6-108">Microsoft support may not be able to assist further.</span></span>
