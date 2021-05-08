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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286695"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potrebujete označiť doménu alebo odosielateľa e-mailu ako dôveryhodnú?

- Neodporúča sa **používať zoznamy dôveryhodných odosielateľov,** pretože sa v organizácii otvárajú útoky na nevyžiadanú poštu, formulácie a predstieranie ich predstierania.
- Ak však existujú obchodné požiadavky, odporúčame vám na **to** používať **[pravidlá Flow pošty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Náš pokyn zabezpečí overovanie odosielateľa (overuje, že odosielaná doména nie je falošný). **Poznámka:** Neodporúčame spravovanie nesprávne pozitívnych správ pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu vašu organizáciu otvoriť pred útokmi zabezpečenia. Ak vaši používateľi dostanú správy, ktoré boli nesprávne označené ako nevyžiadaná pošta alebo nevyžiadaná pošta, správy a súbory **[nahláste spoločnosti Microsoft.](https://protection.office.com/reportsubmission)**
- Trezor Odosielateľom v Outlook, zozname povolených odosielateľov alebo v  zozname povolených domén v politike ochrany pred nevyžiadanou poštou sa treba vyhnúť, pretože odosielatelia obídu všetky ochrany pred nevyžiadanou poštou, predstieraniu odosielateľa a predstieraniu odosielateľa a overeniu odosielateľa (SPF, DKIM, DMARC). Táto metóda je najlepšie používať len na dočasné testovanie.
- Overenie, či je možné vykonať určité vyhodnotenie antispamových obídených e-mailov kontrolou hlavičky správy X-Forefront-Antispam-Report (SFV:SFE, SFV:SKA, SFV:SKN), pozrite si časť Hlavičky správ na ochranu pred **[nevyžiadanou](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** poštou.
- Keďže spoločnosť Microsoft chce predvolene zabezpečiť našich [zákazníkov,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)niektoré prepísania nájomníkov sa nebudú používať pre malvér a neoprávnené získavanie údajov s vysokou spoľahlivosťou. Medzi tieto prepísania patria: o Povolené zoznamy odosielateľov alebo povolené zoznamy domén (politiky ochrany pred nevyžiadanou poštou) o Outlook Trezor zoznam povolených IP adries (filtrovanie pripojenia) 
- Jediné prepísanie, ktoré umožňuje správe s vysokým dôverovaním neoprávneného získavania údajov obísť filtrovanie, je Exchange toku pošty (známe aj ako pravidlá prenosu). Ak chcete použiť pravidlá toku pošty na obídenie filtrovania, pozrite si časť Použitie pravidiel toku pošty na nastavenie úrovne **[spoľahlivosti nevyžiadanej](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** pošty v správach.