---
title: Prijímanie poštových schránok s obmedzením presadzovania
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316035"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Prijímanie poštových schránok s obmedzením presadzovania

Spoločnosť Microsoft nedávno začala vynútenie prahovej hodnoty 3600 správ za hodinu na jednu poštovú schránku. Ďalšie informácie nájdete v téme [Exchange Online limity.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 schránok, ktoré do hodiny dostávajú viac ako 3 600 správ, sú na nasledujúcich 60 minút obmedzenia. 

Okrem toho sa použije limit párov odosielateľov a príjemcov (SRP), ktorý blokuje správy prijaté Microsoft 365 od konkrétneho odosielateľa. Ak jeden odosielateľ odošle konkrétnemu príjemcovi viac ako 33 % z celkovej prahovej hodnoty alebo 1 200 správ za priebehu jednej hodiny, otvorí sa limit počturpov a poštová schránka už nebude prijímať správy od tohto odosielateľa. Všimnite si, že:

- Tento limit sa používa na e-maily prijaté od iných nájomníkov, lokálnych alebo internetových odosielateľov.
- Doručovanie e-mailov do poštovej schránky je blokované na ďalších 60 minút. 
- Odosielatelia týchto poštových schránok dostanú správu o doručení (5.2.121 alebo 5.2.122) s informáciami, že poštová schránka prekročila maximálnu veľkosť doručenia. Intra-tenant (pošta v rámci toho istého nájomníka) sa naďalej doručí.
- Po použití limitu SRP prijímaná poštová schránka naďalej prijíma správy od iných odosielateľov.

Správcovia môžu sledovať aktuálnu aktivitu poštovej schránky prostredníctvom prístupu k novej zostave a prehľadu v Centre spravovania služby Exchange s názvom Poštové schránky prekračujúce limity prijímania. Prehľad sa zobrazí iba v prípade, že nájomník má neuhradenú poštovú schránka, zatiaľ čo zostava sa vždy zobrazuje na tabuli, ale je prázdna, pokiaľ nájomník nemá neuhradenú poštovú schránka.

Ďalšie informácie o limitoch prijímania prehľadov nájdete v téme Poštové schránky [s prehľadom o prekročení limitov v novom EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Ďalšie informácie o správe o prekročení prijímajúcich limitov nájdete v správe o prekročenie limitov prijímania poštových [schránok v novom EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)