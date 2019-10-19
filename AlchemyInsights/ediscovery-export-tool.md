---
title: nástroj na export eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736340"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nie je možné nainštalovať alebo spustiť nástroj na export eDiscovery?

Ak nemôžete nainštalovať alebo spustiť Office 365 eDiscovery Export nástroj na stiahnutie výsledkov vyhľadávania, skontrolujte nasledujúce veci:
  
- Počítač, ktorý používate, spĺňa tieto predpoklady:

  - 32-alebo 64-bitové verzie systému Windows 7 a novšie verzie

  - Microsoft .NET Framework 4,7

  - Podporovaný prehliadač:

  - Microsoft Edge

    Alebo

  - Internet Explorer 10 a novšie verzie

    Iné prehliadače, napríklad Google Chrome a Mozilla Firefox, nie sú podporované.

- Vaša organizácia sa môže pripojiť k koncový bod v Azure, ktorý je ** \*. blob.Core.Windows.net** (zástupný znak predstavuje Jednoznačný identifikátor pre vašu úlohu exportu).

- Priradíte rolu exportu v centre zabezpečenia &amp; Office 365. Táto rola je predvolene priradená len skupine rolí eDiscovery Manager. Pozrite si [Priradenie povolení eDiscovery](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Ďalšie informácie nájdete v téme [exportovanie výsledkov vyhľadávania obsahu](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  