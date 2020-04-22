---
title: Antispam-5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676512"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="a4fe2-102">Oprava problémov s doručením e-mailu pre kód chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="a4fe2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="a4fe2-103">Skontrolujte záznam SPF DNS pre vašu doménu na verejne dostupnej SPF alebo DNS záznam Checker na webe.</span><span class="sxs-lookup"><span data-stu-id="a4fe2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="a4fe2-104">Overte, či odchádzajúca správa nebola identifikovaná ako spam spoločnosťou Microsoft a smerovaná cez [vysoko rizikové dodanie fondu](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="a4fe2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="a4fe2-105">Správy v bazéne s vysokým rizikom neprejdú SPF kontroly, a preto nebude prijatý cieľovej e-mailovej organizácie.</span><span class="sxs-lookup"><span data-stu-id="a4fe2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="a4fe2-106">Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ku ktorému sa pokúšate Odoslať e-mail.</span><span class="sxs-lookup"><span data-stu-id="a4fe2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="a4fe2-107">Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku.</span><span class="sxs-lookup"><span data-stu-id="a4fe2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="a4fe2-108">Podpora spoločnosti Microsoft nemusí byť schopná pomôcť ďalej.</span><span class="sxs-lookup"><span data-stu-id="a4fe2-108">Microsoft support may not be able to assist further.</span></span>
