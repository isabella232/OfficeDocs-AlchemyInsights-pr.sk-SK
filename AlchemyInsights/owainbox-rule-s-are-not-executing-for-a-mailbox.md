---
title: 1332 OWA – Pravidlá pre doručenú poštu sa pre poštovú schránku neslúnia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040917"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo pre doručenú poštu nefunguje podľa očakávania

Skontrolujte tieto nastavenia v Outlook na webe:

- Správu možno presmerovať, preposlať alebo na ktorú môžete automaticky odpovedať na základe pravidiel pre doručenú poštu iba raz. Pravidlo presmerovania (pravidlo pre doručenú poštu alebo pravidlo toku pošty, známe aj ako pravidlo prenosu) môže do správy pridať maximálne desať príjemcov presmerovania. Ďalšie informácie nájdete v téme Obmedzenia [pravidiel Denník, Prenos a Doručená pošta.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Pravidlá pre doručenú poštu v alternatívnej poštovej schránke denníka nefungujú. Ďalšie informácie o alternatívnej poštovej schránke denníka nájdete v téme Alternatívna [poštová schránka denníka.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Ak chcete tieto problémy vyriešiť, pozrite si [článok vedomostnej databázy 2829319](https://support.microsoft.com/kb/2829319).

Ak sa predchádzajúce problémy nevzťahujú, skôr než sa problém presunete na technickú podporu spoločnosti Microsoft, spustite diagnostickú zostavu pravidla pre doručenú poštu:

1. Otvorte poštovú schránku v Outlook na webe a kliknite na položku <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavenia**  >  **Zobraziť všetky Outlook Nastavenia**  >  **Pošta**  >  **Pravidlá.**

2. V dolnej časti stránky kliknite na položku Ak vaše pravidlá nefungujú, kliknutím sem **vygenerujte zostavu diagnostiky.**
