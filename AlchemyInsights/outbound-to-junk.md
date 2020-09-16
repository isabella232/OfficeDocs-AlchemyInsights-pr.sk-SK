---
title: Odchádzajúce e-maily do priečinka Nevyžiadaná pošta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769198"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="b484c-102">Odchádzajúce e-maily do priečinka Nevyžiadaná pošta</span><span class="sxs-lookup"><span data-stu-id="b484c-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="b484c-103">Ak sa zobrazujú odchádzajúce správy označené ako nevyžiadané, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="b484c-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="b484c-104">Ak ste tak ešte neurobili, zvážte možnosť [konfigurácie oznámení o politike odchádzajúcej pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="b484c-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="b484c-105">Použite [sledovanie správ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) a zistite, či výstupná správa obsahuje **nevyžiadanú poštu** v hodnote udalosti s ďalšími detailmi: **použite fond s vysokým rizikom doručenia**.</span><span class="sxs-lookup"><span data-stu-id="b484c-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="b484c-106">Pri týchto správach skontrolujte obsah správy a zistite, čo môže byť považované za nevyžiadanú poštu.</span><span class="sxs-lookup"><span data-stu-id="b484c-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="b484c-107">Podpisy môžu napríklad niekedy spôsobovať problémy pre mnohých používateľov.</span><span class="sxs-lookup"><span data-stu-id="b484c-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="b484c-108">Ak máte viacero príkladov oprávnených odchádzajúcich správ, ktoré sú označené ako nevyžiadané, otvorte lístok technickej podpory a požiadajte agenta podpory, aby odoslal správy ako falošné pozitívy pre našich analytikov nevyžiadanej pošty.</span><span class="sxs-lookup"><span data-stu-id="b484c-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="b484c-109">Buďte pripravení poskytnúť vzorové správy, ktoré obsahujú všetky hlavičky správ.</span><span class="sxs-lookup"><span data-stu-id="b484c-109">Be prepared to provide sample messages that include all message headers.</span></span>
