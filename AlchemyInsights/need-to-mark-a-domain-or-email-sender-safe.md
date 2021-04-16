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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potrebujete označiť doménu alebo odosielateľa e-mailu ako dôveryhodnú?

- Neodporúča sa **používať zoznamy dôveryhodných odosielateľov,** pretože sa v organizácii otvárajú útoky na nevyžiadanú poštu, formulácie a predstieranie ich predstierania.
- Ak však existujú obchodné požiadavky, odporúčame **v** tomto prípade používať pravidlá **[toku](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošty. Náš pokyn zabezpečí overovanie odosielateľa (overuje, že odosielaná doména nie je falošný). **Poznámka:** Neodporúčame spravovanie nesprávne pozitívnych správ pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu vašu organizáciu otvoriť pred útokmi zabezpečenia. Ak vaši používateľi dostanú správy, ktoré boli nesprávne označené ako nevyžiadaná pošta alebo nevyžiadaná pošta, správy a súbory **[nahláste spoločnosti Microsoft.](https://protection.office.com/reportsubmission)**
- Zoznamu dôveryhodných odosielateľov v Outlooku, zozname povolených  odosielateľov alebo v zozname povolených domén v politike ochrany pred nevyžiadanou poštou sa treba vyhnúť, pretože odosielatelia obídu všetky ochrany pred nevyžiadanou poštou, predstieraniu odosielateľa a predstieraniu odosielateľa (SPF, DKIM, DMARC). Táto metóda je najlepšie používať len na dočasné testovanie.
