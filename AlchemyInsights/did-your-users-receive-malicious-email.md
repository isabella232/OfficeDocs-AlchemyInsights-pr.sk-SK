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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815261"
---
# <a name="did-your-users-receive-malicious-email"></a>Dostali vaši používatelia škodlivé e-maily?

- Teraz môžete škodlivé e-maily nahlásiť spoločnosti Microsoft pomocou [Odoslaní, ktoré vykonal správca, v centre zabezpečenia a dodržiavania súladu](https://sip.protection.office.com/reportsubmission).

Správy [odoslané správcom](https://sip.protection.office.com/reportsubmission) sú skontrolované a výsledky sa zobrazia v zobrazení **detailov**:

- Ak sa pri doručení vyskytlo zlyhanie overenia e-mailu odosielateľa.
- Informácie o nálezoch politiky, ktoré mohli ovplyvniť alebo prepísať verdikt správy.
- Aktuálne výsledky detonácie na zistenie toho, či adresy URL v správe boli nebezpečné alebo nie.
- Pripomienky od hodnotiteľov

Ak sa našlo prepísanie, opätovná kontrola by sa mala dokončiť za niekoľko minút. Ak sa s e-mailovým overovaním nevyskytol žiadny problém alebo ak doručenie nebolo ovplyvnené prepísaním, pripomienky od hodnotiteľov môžu prísť až o deň.

Ak nesúhlasíte s konečným verdiktom týkajúcim sa správy, URL adresy alebo súboru (blokovaný alebo neblokovaný), správu odošlite o deň na opätovnú kontrolu. Je veľmi pravdepodobné, že vedikt sa po opätovnom odoslaní správy zmení.

Medzitým môžete odstrániť škodlivé e-maily z prijatej pošty používateľov pomocou inštrukcií v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Zákazníci s Microsoft Defender pre Office 365 môžu:
    - použiť [Prieskumníka hrozieb na nájdenie a odstránenie podozrivých e-mailov](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [používať bezpečné prepojenia na blokovanie prístupu](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) k škodlivej URL adrese
    - sledovať používateľov, ktorí klikli a prešli na škodlivé URL adresy: [Zobraziť URL adresy zamerané na neoprávnené získavanie údajov](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Získať UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ručne [spustiť automatizované skúmanie](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Chrániť pred škodlivými súbormi a URL adresami môžete tiež pomocou krokov uvedených v časti [Ochrana pred škodlivými URL adresami a súbormi](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).