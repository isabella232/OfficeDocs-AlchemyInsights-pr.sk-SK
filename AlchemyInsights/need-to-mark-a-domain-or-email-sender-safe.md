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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potrebujete označenie domény alebo odosielateľa e-mailu v bezpečí?

- Používanie **zoznamov dôveryhodných odosielateľov sa neodporúča** , pretože otvára svoju organizáciu na nevyžiadanú poštu, Phish a spoofing.
- Ak však existujú obchodné požiadavky, **odporúčame** použiť **[pravidlá toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Naše usmernenie zabezpečuje overenie odosielateľa (overí, že odosielajúca doména nie je falošná). **Poznámka**: Neodporúčame spravovanie falošných poplachov pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu otvoriť vašu organizáciu prostredníctvom bezpečnostných útokov. Ak používatelia prijímajú správy nesprávne označené ako nevyžiadaná pošta alebo Nevyžiadaná pošta, **[nahláste správy a súbory do spoločnosti Microsoft](https://protection.office.com/reportsubmission)**.
- Dôveryhodní odosielatelia v Outlooku, povolený zoznam odosielateľov alebo povolený zoznam domén v politikách ochrany pred nevyžiadanou poštou **by sa mali vyhnúť** , pretože odosielatelia obchádzajú všetky nevyžiadanú poštu, spoof a ochranu Phish a overenie odosielateľa (SPF, DKIM, DMARC). Táto metóda sa používa len na dočasné testovanie.
