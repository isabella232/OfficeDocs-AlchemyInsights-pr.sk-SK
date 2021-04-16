---
title: Nástroj na exportovanie eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814603"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nemôžete nainštalovať alebo spustiť nástroj na exportovanie eDiscovery?

Ak nemôžete nainštalovať alebo spustiť nástroj na exportovanie eDiscovery a stiahnuť výsledky vyhľadávania, skontrolujte tieto veci:
  
- Počítač, ktorý používate, spĺňa tieto požiadavky:

  - 32-bitová alebo 64-bitová verzia Windowsu 7 a novšie verzie

  - Microsoft .NET Framework 4.7

  - Podporovaný prehliadač:

  - Microsoft Edge

    Alebo

  - Internet Explorer 10 a novšie verzie

    Iné prehliadače, napríklad Google Chrome a Mozilla Firefox, nie sú podporované.

- Vaša organizácia sa môže pripojiť ku koncovmu bodu v službe Azure, čo je **\* .blob.core.windows.net** (zástupný znak predstavuje jedinečný identifikátor úlohy exportu).

- V Centre zabezpečenia služieb Microsoft 365 máte priradenú rolu &amp; exportu. Táto rola je predvolene priradená len skupine rolí eDiscovery Manager. Pozrite si [časť Priradenie povolení na eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Ďalšie informácie nájdete v téme [Export výsledkov vyhľadávania obsahu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Ak exportujete viac ako 100 000 poštových schránok, na stiahnutie výsledkov exportu budete musieť použiť toto prostredie PowerShell: Export výsledkov z viac ako  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)poštových schránok.