---
title: Vyhľadávanie obsahu bez výsledkov
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816863"
---
# <a name="no-results-from-content-searchexports"></a>Žiadne výsledky vyhľadávania a exportov obsahu

Problémy s vyhľadávaním a exportmi obsahu, pri ktorých sa vracajú žiadne údaje, môže spôsobovať určitý filter zabezpečenia súladu, ktorý nastavuje konkrétny správca a ktorý ho nekomunikuje všetkým správcom.

Ak chcete vyriešiť tento problém, skontrolujte, či to môžu spôsobovať niektoré filtre zabezpečenia súladu:
1. Pripojenie k centre zabezpečenia a dodržiavania súladu v prostredí Powershell
2. Spustite nasledujúce commandlety:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – Organizácia $org