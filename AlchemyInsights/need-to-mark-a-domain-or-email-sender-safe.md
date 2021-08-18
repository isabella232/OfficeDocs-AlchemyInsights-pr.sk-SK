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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319963"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potrebujete označiť doménu alebo odosielateľa e-mailu ako dôveryhodnú?

- Neodporúča sa **používať zoznamy dôveryhodných odosielateľov,** pretože sa v organizácii otvárajú útoky na nevyžiadanú poštu, formulácie a predstieranie ich predstierania.
- Ak však existujú obchodné požiadavky, odporúčame vám na **to** používať **[pravidlá Flow pošty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Náš pokyn zabezpečí overovanie odosielateľa (overuje, že odosielaná doména nie je falošný). 
    **Poznámka:** Neodporúčame spravovanie nesprávne pozitívnych správ pomocou zoznamov dôveryhodných odosielateľov, pretože výnimky z filtrovania nevyžiadanej pošty môžu vašu organizáciu otvoriť pred útokmi zabezpečenia. Ak vaši používateľi dostanú správy, ktoré boli nesprávne označené ako nevyžiadaná pošta alebo nevyžiadaná pošta, **[nahlásenie správ a súborov spoločnosti Microsoft.](https://protection.office.com/reportsubmission)**
- Trezor Odosielateľom v Outlook, zozname povolených odosielateľov alebo v zozname  povolených domén v politike ochrany pred nevyžiadanou poštou sa treba vyhnúť, pretože odosielatelia obídu všetky ochrany pred nevyžiadanou poštou, predstieraniu odosielateľa a predstieraniu odosielateľa (SPF, DKIM, DMARC). Táto metóda je najlepšie používať len na dočasné testovanie.
- Overenie, že určité vyhodnotenie antispamu obíde e-mailu pomocou kontroly hlavičky správy X-Forefront-Antispam-Report (SFV:SFE, SFV:SKA, SFV:SKN), nájdete v téme Hlavičky správ na ochranu pred **[nevyžiadanou](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** poštou.
- Keďže spoločnosť Microsoft chce predvolene zabezpečiť našich [zákazníkov,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)niektoré prepísania nájomníkov sa nebudú používať na malvér a neoprávnené získavanie údajov s vysokou spoľahlivosťou. Medzi tieto prepísania patria: o zoznamy povolených odosielateľov alebo povolené zoznamy domén (politiky ochrany pred nevyžiadanou poštou) o Outlook Trezor zoznam povolených ip adries odosielateľov (filtrovanie pripojenia) 
- Jediné prepísanie, ktoré umožňuje správe s vysokým dôverovaním neoprávneného získavania údajov obísť Exchange toku pošty (známe aj ako pravidlá prenosu). Ak chcete použiť pravidlá toku pošty na obídenie filtrovania, pozrite si časť Použitie pravidiel toku pošty na nastavenie úrovne **[spoľahlivosti nevyžiadanej](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** pošty v správach.