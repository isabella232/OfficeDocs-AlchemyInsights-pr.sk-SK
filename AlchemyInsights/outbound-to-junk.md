---
title: Odchádzajúce e-maily do priečinka nevyžiadanej pošty
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761183"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="80048-102">Odchádzajúce e-maily do priečinka nevyžiadanej pošty</span><span class="sxs-lookup"><span data-stu-id="80048-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="80048-103">Ak sa zobrazujú odchádzajúce správy označené ako nevyžiadané, postupujte podľa nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="80048-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="80048-104">Ak ste tak ešte neurobili, zvážte [konfiguráciu odchádzajúcich upozornení politiky nevyžiadanej pošty](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="80048-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="80048-105">Pomocou [sledovania správ](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) Zistite, či odchádzajúca správa má hodnotu udalosti **spam** s dodatočnou podrobnosťou: **použite vysoko rizikové dodávky bazén**.</span><span class="sxs-lookup"><span data-stu-id="80048-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="80048-106">V prípade týchto správ skontrolujte obsah správy a zistite, čo sa môže považovať za spam.</span><span class="sxs-lookup"><span data-stu-id="80048-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="80048-107">Napríklad podpisy môžu niekedy spôsobiť problémy pre mnohých používateľov.</span><span class="sxs-lookup"><span data-stu-id="80048-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="80048-108">Ak máte viacero príkladov legitímnych odchádzajúcich správ, ktoré sú označené ako nevyžiadané, otvorte lístok podpory a požiadajte agenta podpory o odoslanie správ ako falošných poplachov našim analytikom nevyžiadanej pošty.</span><span class="sxs-lookup"><span data-stu-id="80048-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="80048-109">Buďte pripravení poskytnúť ukážkové správy, ktoré obsahujú všetky hlavičky správ.</span><span class="sxs-lookup"><span data-stu-id="80048-109">Be prepared to provide sample messages that include all message headers.</span></span>
