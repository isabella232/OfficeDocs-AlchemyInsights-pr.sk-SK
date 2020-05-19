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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potrebujete označiť doménu alebo odosielateľa e-mailu v bezpečí?

- Použitie **zoznamov bezpečných** odosielateľov sa neodporúča, pretože otvára vašu organizáciu na spam, Phish a falšovanie útokov.
- Avšak, ak je obchodná požiadavka, **odporúčame** použiť **[pravidlá toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pre tento. Naše pokyny zaručujú overenie odosielateľa (overuje sa odosielajúca doména nie je falošná). **Poznámka**: Neodporúčame spravovanie falošných poplachov pomocou zoznamov bezpečných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu otvoriť vašu organizáciu pre bezpečnostné útoky. Ak používateľ (y) dostane správy nesprávne označené ako spam alebo Nevyžiadaná pošta, **[nahláste správy a súbory spoločnosti Microsoft](https://protection.office.com/reportsubmission)**.
- Dôveryhodní odosielatelia v programe Outlook, zoznam povolených odosielateľov alebo povolený zoznam domén v politikách proti spamu **je potrebné sa vyhnúť** , pretože odosielatelia obchádzajú všetok spam, spoof a Phish Protection a overenie odosielateľa (SPF, DKIM, DMARC). Táto metóda sa najlepšie používa len na dočasné testovanie.
