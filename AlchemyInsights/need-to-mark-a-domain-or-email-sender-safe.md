---
title: Potrebujete označiť doménu alebo odosielateľa e-mailu ako dôveryhodnú?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792147"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="7d263-102">Potrebujete označiť doménu alebo odosielateľa e-mailu ako dôveryhodnú?</span><span class="sxs-lookup"><span data-stu-id="7d263-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="7d263-103">Neodporúča sa **používať zoznamy dôveryhodných odosielateľov,** pretože sa v organizácii otvárajú útoky na nevyžiadanú poštu, formulácie a predstieranie ich predstierania.</span><span class="sxs-lookup"><span data-stu-id="7d263-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="7d263-104">Ak však existujú obchodné požiadavky, odporúčame **v** tomto prípade používať pravidlá **[toku](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošty.</span><span class="sxs-lookup"><span data-stu-id="7d263-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="7d263-105">Náš pokyn zabezpečí overovanie odosielateľa (overuje, že odosielaná doména nie je falošný).</span><span class="sxs-lookup"><span data-stu-id="7d263-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="7d263-106">**Poznámka:** Neodporúčame spravovanie nesprávne pozitívnych správ pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu vašu organizáciu otvoriť pred útokmi zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="7d263-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="7d263-107">Ak vaši používateľi dostanú správy, ktoré boli nesprávne označené ako nevyžiadaná pošta alebo nevyžiadaná pošta, správy a súbory **[nahláste spoločnosti Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="7d263-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="7d263-108">Zoznamu dôveryhodných odosielateľov v Outlooku, zozname povolených  odosielateľov alebo v zozname povolených domén v politike ochrany pred nevyžiadanou poštou sa treba vyhnúť, pretože odosielatelia obídu všetky ochrany pred nevyžiadanou poštou, predstieraniu odosielateľa a predstieraniu odosielateľa (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="7d263-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="7d263-109">Táto metóda je najlepšie používať len na dočasné testovanie.</span><span class="sxs-lookup"><span data-stu-id="7d263-109">This method is best used for temporary testing only.</span></span>
