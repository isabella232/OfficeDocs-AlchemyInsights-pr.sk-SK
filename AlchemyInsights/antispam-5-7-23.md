---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717340"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="fd54e-102">Riešenie problémov s doručovaním e-mailov s kódom chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="fd54e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="fd54e-103">Overte záznam SPF DNS pre svoju doménu na verejne dostupnej kontrole záznamov SPF alebo DNS na webe.</span><span class="sxs-lookup"><span data-stu-id="fd54e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="fd54e-104">Overte, či výstupná správa nebola identifikovaná spoločnosťou Microsoft ako nevyžiadaná pošta, a smerovala cez [bazén s vysokým rizikom](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="fd54e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="fd54e-105">Správy v bazéne s vysokým rizikom neprejdú kontrolou SPF, a preto nebudú akceptované cieľovou e-mailovou organizáciou.</span><span class="sxs-lookup"><span data-stu-id="fd54e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="fd54e-106">Ak problém pretrváva, možno bude potrebné obrátiť sa na správcu hostiteľa pošty, ku ktorému sa pokúšate Odoslať e-mail.</span><span class="sxs-lookup"><span data-stu-id="fd54e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="fd54e-107">Poznačte si podrobnú externú chybu dostupnú v správe Bounce.</span><span class="sxs-lookup"><span data-stu-id="fd54e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="fd54e-108">Technická podpora spoločnosti Microsoft nemusí byť schopná poskytnúť ďalšiu pomoc.</span><span class="sxs-lookup"><span data-stu-id="fd54e-108">Microsoft support may not be able to assist further.</span></span>
