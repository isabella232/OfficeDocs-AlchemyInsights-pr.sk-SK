---
title: Dostali vaši používatelia škodlivé e-maily
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326722"
---
# <a name="did-your-users-receive-malicious-email"></a>Dostali vaši používatelia škodlivé e-maily?

Škodlivé e-maily môžete teraz spoločnosti Microsoft nahlásiť [pomocou odoslania na Microsoft 365 Defender portáli](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Správy odoslané v [odoslaných správach správcu sa](https://security.microsoft.com/reportsubmission?viewid=admin) skenujú a v detailnej bubline sa zobrazia nasledujúce výsledky:

- Ak sa pri doručení vyskytlo zlyhanie overenia e-mailu odosielateľa.
- Informácie o nálezoch politiky, ktoré mohli ovplyvniť alebo prepísať verdikt správy.
- Aktuálne výsledky detonácie na zistenie toho, či adresy URL v správe boli nebezpečné alebo nie.
- Pripomienky od hodnotiteľov

Ak sa našlo prepísanie, opätovná kontrola by sa mala dokončiť za niekoľko minút. Ak sa s e-mailovým overovaním nevyskytol žiadny problém alebo ak doručenie nebolo ovplyvnené prepísaním, pripomienky od hodnotiteľov môžu prísť až o deň.

Ak nesúhlasíte s konečným verdiktom týkajúcim sa správy, URL adresy alebo súboru (blokovaný alebo neblokovaný), správu odošlite o deň na opätovnú kontrolu. Je veľmi pravdepodobné, že vedikt sa po opätovnom odoslaní správy zmení.

Medzitým môžete odstrániť škodlivé e-maily z prijatej pošty používateľov pomocou inštrukcií v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Zákazníci s Microsoft Defender pre Office 365 môžu:
  - Vyhľadanie [a odstránenie podozrivých e-mailov pomocou Prieskumníka hrozieb](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Blokovanie Trezor a zlomyseľných URL adries](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) pomocou prepojení na webové lokality
  - Sledovanie používateľov, ktorí klikli na škodlivé URL adresy a pristupovali k nim: Zobrazte [URL adresu neoprávneného](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)získavania údajov a kliknite na položku údaje  &  [verdict Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Manuálne [spustenie automatizovaného skúmania](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Chrániť pred škodlivými súbormi a URL adresami môžete tiež pomocou krokov uvedených v časti [Ochrana pred škodlivými URL adresami a súbormi](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
