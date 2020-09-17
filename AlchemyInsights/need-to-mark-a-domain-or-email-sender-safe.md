---
title: Potrebujete označenie domény alebo odosielateľa e-mailu v bezpečí?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803260"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="8a25f-102">Potrebujete označenie domény alebo odosielateľa e-mailu v bezpečí?</span><span class="sxs-lookup"><span data-stu-id="8a25f-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="8a25f-103">Používanie **zoznamov dôveryhodných odosielateľov sa neodporúča** , pretože otvára svoju organizáciu na nevyžiadanú poštu, Phish a spoofing.</span><span class="sxs-lookup"><span data-stu-id="8a25f-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="8a25f-104">Ak však existujú obchodné požiadavky, **odporúčame** použiť **[pravidlá toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="8a25f-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="8a25f-105">Naše usmernenie zabezpečuje overenie odosielateľa (overí, že odosielajúca doména nie je falošná).</span><span class="sxs-lookup"><span data-stu-id="8a25f-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="8a25f-106">**Poznámka**: Neodporúčame spravovanie falošných poplachov pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu otvoriť vašu organizáciu prostredníctvom bezpečnostných útokov.</span><span class="sxs-lookup"><span data-stu-id="8a25f-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="8a25f-107">Ak používatelia prijímajú správy nesprávne označené ako nevyžiadaná pošta alebo Nevyžiadaná pošta, **[nahláste správy a súbory do spoločnosti Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="8a25f-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="8a25f-108">Dôveryhodní odosielatelia v Outlooku, povolený zoznam odosielateľov alebo povolený zoznam domén v politikách ochrany pred nevyžiadanou poštou **by sa mali vyhnúť** , pretože odosielatelia obchádzajú všetky nevyžiadanú poštu, spoof a ochranu Phish a overenie odosielateľa (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="8a25f-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="8a25f-109">Táto metóda sa používa len na dočasné testovanie.</span><span class="sxs-lookup"><span data-stu-id="8a25f-109">This method is best used for temporary testing only.</span></span>
