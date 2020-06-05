---
title: 1332 OWA - doručenej pošty pravidlá nie sú vykonávajúci poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576575"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo doručenej pošty nefunguje podľa očakávania

Skontrolujte nasledujúce nastavenia v Outlooku na webe:

- Správu je možné presmerovať, poslať ďalej alebo odpovedať automaticky na základe pravidiel pre doručenú poštu iba raz. Pravidlo presmerovania (pravidlo pre doručenú poštu alebo pravidlo toku pošty, známe aj ako pravidlo prenosu) môže do správy pridať maximálne desať príjemcov posielania ďalej. Ďalšie informácie sa nachádzajú v téme [Limity pravidiel denníkov, dopravy a doručenej pošty](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravidlá pre doručenú poštu nefungujú v alternatívnej poštovej schránke denníka. Ďalšie informácie o alternatívnej poštovej schránke denníka nájdete v téme [Alternatívne zapisovanie do denníka poštovej schránky](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Ak chcete vyriešiť tieto problémy, pozrite si [KB 2829319](https://support.microsoft.com/kb/2829319).

Ak sa nepoužijú predchádzajúce problémy, pred eskaláciou problému technickej podpore spoločnosti Microsoft spustite diagnostickú správu pravidla doručenej pošty:

1. Otvorte poštovú schránku v Outlooku na webe a kliknite na tlačidlo <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavenia (Settings)**  >  **Zobraziť všetky nastavenia**  >  programu Outlook **Poštová schránka**  >  **pravidlá .**

2. V dolnej časti stránky kliknite na položku **Ak pravidlá nefungujú, kliknite sem a vygenerujte diagnostickú správu**.
