---
title: Potrebujete označiť doménu alebo odosielateľa e-mailu v bezpečí?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281186"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="8c7ae-102">Potrebujete označiť doménu alebo odosielateľa e-mailu v bezpečí?</span><span class="sxs-lookup"><span data-stu-id="8c7ae-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="8c7ae-103">Použitie **zoznamov bezpečných** odosielateľov sa neodporúča, pretože otvára vašu organizáciu na spam, Phish a falšovanie útokov.</span><span class="sxs-lookup"><span data-stu-id="8c7ae-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="8c7ae-104">Avšak, ak je obchodná požiadavka, **odporúčame** použiť **[pravidlá toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pre tento.</span><span class="sxs-lookup"><span data-stu-id="8c7ae-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="8c7ae-105">Naše pokyny zaručujú overenie odosielateľa (overuje sa odosielajúca doména nie je falošná).</span><span class="sxs-lookup"><span data-stu-id="8c7ae-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="8c7ae-106">**Poznámka**: Neodporúčame spravovanie falošných poplachov pomocou zoznamov bezpečných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu otvoriť vašu organizáciu pre bezpečnostné útoky.</span><span class="sxs-lookup"><span data-stu-id="8c7ae-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="8c7ae-107">Ak používateľ (y) dostane správy nesprávne označené ako spam alebo Nevyžiadaná pošta, **[nahláste správy a súbory spoločnosti Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="8c7ae-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="8c7ae-108">Dôveryhodní odosielatelia v programe Outlook, zoznam povolených odosielateľov alebo povolený zoznam domén v politikách proti spamu **je potrebné sa vyhnúť** , pretože odosielatelia obchádzajú všetok spam, spoof a Phish Protection a overenie odosielateľa (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="8c7ae-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="8c7ae-109">Táto metóda sa najlepšie používa len na dočasné testovanie.</span><span class="sxs-lookup"><span data-stu-id="8c7ae-109">This method is best used for temporary testing only.</span></span>
