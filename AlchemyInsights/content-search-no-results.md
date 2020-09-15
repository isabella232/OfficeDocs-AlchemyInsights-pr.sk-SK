---
title: Vyhľadávanie obsahu žiadne výsledky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680662"
---
# <a name="no-results-from-content-searchexports"></a>Žiadne výsledky z vyhľadávania obsahu alebo exportu

Problémy s vyhľadávaním obsahu alebo exportovaním, ktoré nevracajú žiadne údaje, môžu byť spôsobené niektorými filtrami zabezpečenia súladu, ktorý bol nastavením konkrétneho správcu, a nekomunikoval ho so všetkými správcami.

Ak chcete tento problém vyriešiť, skontrolujte, či sa nenachádzajú žiadne filtre zabezpečenia dodržiavania súladu, ktoré môžu spôsobovať toto:
1. Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu
2. Spustite nasledovné príkazové aplety:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizácia $org