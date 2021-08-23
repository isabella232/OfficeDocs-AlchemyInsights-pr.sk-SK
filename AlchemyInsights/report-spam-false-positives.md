---
title: Chcete spoločnosti Microsoft nahlásiť nevyžiadanú poštu s nesprávne pozitívnym nádychom?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396630"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Označujú sa vám legitímne správy ako nevyžiadaná pošta?

Legitímne e-maily sa končia v priečinku Nevyžiadaná pošta alebo v karanténe, čo je frustrujúce. Zvážte tieto najbežnejšie dôvody pre nesprávne pozitívne výsledky:

**Prepísania nájomníkov (najčastejšie)** Tento problém je plne pod kontrolou na opravenie.

odošlite správu na Microsoft 365 Defender analýzy ovplyvňujúce politiky a pravidlá, Podrobnosti rescan sú k dispozícii v priebehu niekoľkých minút.
Skontrolujte alebo upravte politiky alebo pravidlá podľa potreby. 

**Prepísania koncovými používateľmi (bežné)** Tento problém je plne pod kontrolou na opravenie. 

odošlite správu na Microsoft 365 Defender analýzy ovplyvňujúce politiky a pravidlá, Podrobnosti rescan sú k dispozícii v priebehu niekoľkých minút. 

Ak bola správa zablokovaná, pretože bola odoslaná z adresy v zozname blokovaných odosielateľov používateľa, hlavičky obsahujú text Verdict "SFV:BLK".

**Overenie e-mailu odosielateľov** Toto je čiastočne vo vašom ovládacom prvku na opravenie.

odošlite správu, ak chcete analyzovať zlyhania pri overovaní e-mailu odosielateľa v čase doručenia, výsledky sú k dispozícii v priebehu jedného dňa. 

Ak vlastníte odosielanú infraštruktúru, skontrolujte, ako ju zjednotiť so SPF, DKIM a DMARC, aby ste sa uistili, že cieľové e-mailové systémy dôverujú správam odoslaým z vašej domény. Prípadne kontaktujte odosielateľov, aby sa obrátili na ich konfiguráciu DNS systému.

**Verdikt filtrovania od spoločnosti Microsoft** Toto je čiastočne vo vašom ovládacom prvku na opravenie.

odošlite správu a správu nahláste ako bezpečnú, Rescan výsledky sú k dispozícii v priebehu dňa. Ak nesúhlasíte s filtrovaním verktov v určitých situáciách, použite zoznam povolených alebo blokovaných nájomníkov. Nemali by ste však natrvalo obísť overovanie filtrovaním od spoločnosti Microsoft. 

Ďalšie informácie nájdete v téme:

- Povoľte koncovým používateľom odosielať správy spoločnosti Microsoft. Spoločnosť Microsoft používa tieto odoslania na zvýšenie efektívnosti technológií na ochranu e-mailov, ktoré sa zobrazia v odoslaných správach, ktoré môžete použiť ako ukazovateľ aktualizácie politík. 

- Ak si chcete pozrieť krátke video o odosielaní správ na analýzu, pozrite si [časť Odoslanie správ na analýzu.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Použitie odoslania správcu na odosielanie podozrivých nevyžiadanej pošty, phish, URL adries a súborov do spoločnosti Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Správa zoznamu povolených alebo blokovaných nájomníkov](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Hlavičky správ na ochranu pred nevyžiadanou poštou Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Ochrana pred odchádzajúca nevyžiadanou poštou v systéme EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)