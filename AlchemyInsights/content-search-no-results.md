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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058017"
---
# <a name="no-results-from-content-searchexports"></a>Žiadne výsledky vyhľadávania a exportov obsahu

Problémy s vyhľadávaním a exportmi obsahu, pri ktorých sa vracajú žiadne údaje, môže spôsobovať určitý filter zabezpečenia súladu, ktorý nastavuje konkrétny správca a ktorý ho nekomunikuje všetkým správcom.

Ak chcete vyriešiť tento problém, skontrolujte, či to môžu spôsobovať niektoré filtre zabezpečenia súladu:
1. Pripojenie prostredia Powershell centra zabezpečenia a dodržiavania súladu
2. Spustite nasledujúce commandlety:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – Organizácia $org