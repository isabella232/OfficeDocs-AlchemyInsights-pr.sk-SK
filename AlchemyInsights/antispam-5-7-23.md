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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682286"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="31b4c-102">Oprava problémov s doručením e-mailu pre kód chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="31b4c-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="31b4c-103">Skontrolujte záznam SPF DNS pre vašu doménu na verejne dostupnej SPF alebo DNS záznam Checker na webe.</span><span class="sxs-lookup"><span data-stu-id="31b4c-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="31b4c-104">Overte, či odchádzajúca správa nebola identifikovaná ako spam v balíku Office 365 a smerovaný cez [vysoko rizikové dodanie fondu](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="31b4c-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="31b4c-105">Správy v bazéne s vysokým rizikom neprejdú SPF kontroly, a preto nebude prijatý cieľovej e-mailovej organizácie.</span><span class="sxs-lookup"><span data-stu-id="31b4c-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="31b4c-106">Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ku ktorému sa pokúšate Odoslať e-mail.</span><span class="sxs-lookup"><span data-stu-id="31b4c-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="31b4c-107">Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku.</span><span class="sxs-lookup"><span data-stu-id="31b4c-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="31b4c-108">Podpora balíka Office 365 nemusí byť schopná pomôcť ďalej.</span><span class="sxs-lookup"><span data-stu-id="31b4c-108">Office 365 support may not be able to assist further.</span></span>