---
title: Žiadne výsledky vyhľadávania obsahu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800586"
---
# <a name="no-results-from-content-searchexports"></a>Žiadne výsledky z obsahu vyhľadávanie/vývoz

Problémy s obsahom Hľadať/vývoz nevracajú žiadne údaje môžu byť spôsobené určité súlad Filter zabezpečenia, ktorý bol konkrétne Admin a nekomunikuje pre všetky adminy.

Ak chcete vyriešiť tento problém, skontrolujte, ak existuje súlad bezpečnostné filtre, ktoré môžu byť príčinou:
1. Pripojiť k bezpečnosti a centrum súladu Powershell
2. Spustite nasledujúce riešenia:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizácia $org