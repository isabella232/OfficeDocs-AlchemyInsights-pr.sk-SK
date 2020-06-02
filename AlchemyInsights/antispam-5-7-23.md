---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506458"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="db37a-102">Riešenie problémov s doručovaním e-mailov s kódom chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="db37a-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="db37a-103">Overte záznam DNS SPF pre svoju doménu pri verejne dostupnej kontrole záznamov SPF alebo DNS na webe.</span><span class="sxs-lookup"><span data-stu-id="db37a-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="db37a-104">Overte, či spoločnosť Microsoft neidentifikovala odchádzajúca správu ako nevyžiadanú poštu a smerovala cez [fond doručovania s vysokým rizikom.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="db37a-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="db37a-105">Správy vo vysokorizikovom fonde doručovania neprejdú kontrolami SPF, a preto ich cieľová e-mailová organizácia neprijme.</span><span class="sxs-lookup"><span data-stu-id="db37a-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="db37a-106">Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ktorému sa pokúšate odoslať e-mail.</span><span class="sxs-lookup"><span data-stu-id="db37a-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="db37a-107">Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku.</span><span class="sxs-lookup"><span data-stu-id="db37a-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="db37a-108">Technická podpora spoločnosti Microsoft nemusí byť schopná ďalej pomáhať.</span><span class="sxs-lookup"><span data-stu-id="db37a-108">Microsoft support may not be able to assist further.</span></span>
