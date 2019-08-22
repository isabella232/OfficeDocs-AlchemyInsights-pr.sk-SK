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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516794"
---
# <a name="no-results-from-content-searchexports"></a>Žiadne výsledky z obsahu vyhľadávanie/vývoz

Problémy s obsahom Hľadať/vývoz nevracajú žiadne údaje môžu byť spôsobené určité súlad Filter zabezpečenia, ktorý bol konkrétne Admin a nekomunikuje pre všetky adminy.

Ak chcete vyriešiť tento problém, skontrolujte, ak existuje súlad bezpečnostné filtre, ktoré môžu byť príčinou:
1. Pripojiť k bezpečnosti a centrum súladu Powershell
2. Spustite nasledujúce riešenia:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizácia $org