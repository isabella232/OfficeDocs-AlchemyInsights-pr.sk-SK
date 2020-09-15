---
title: 1332 OWA – pravidla pre doručenú poštu sa nevykonávajú pre poštovú schránku
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
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721606"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo doručenej pošty nefunguje podľa očakávaní

Overte nasledujúce nastavenia v Outlooku na webe:

- Správu možno presmerovať, preposlať alebo odpovedať automaticky na základe pravidiel pre doručenú poštu len raz. Pravidlo presmerovania (pravidlo pre doručenú poštu alebo pravidlo toku pošty, ktoré sa označuje aj ako pravidlo prenosu), môže do správy pridať maximálne 10 preposielaných príjemcov. Ďalšie informácie nájdete v téme [limity pravidiel denník, doprava a Doručená pošta](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravidlá pre doručenú poštu nefungujú v poštovej schránke s alternatívnymi denníkmi. Ďalšie informácie o poštovej schránke s alternatívnymi denníkmi nájdete v téme [alternatívny denník poštovej schránky](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Ak chcete vyriešiť tieto problémy, pozrite si tému [KB 2829319](https://support.microsoft.com/kb/2829319).

Ak sa predchádzajúce problémy nepoužijú, pred vykonaním vyriešenia problému na oddelenie technickej podpory spoločnosti Microsoft Spustite diagnostickú zostavu pravidiel pre doručenú poštu:

1. Otvorte poštovú schránku v Outlooku na webe a kliknite na položku <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavenia**  >  **Zobrazenie všetkých nastavení**  >  Outlooku **Pošta**  >  **Pravidlá**.

2. V dolnej časti stránky kliknite na položku **Ak vaše pravidlá nefungujú, kliknite sem, ak chcete vytvoriť diagnostickú zostavu**.
