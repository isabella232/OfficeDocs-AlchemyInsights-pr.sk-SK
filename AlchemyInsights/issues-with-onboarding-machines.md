---
title: Problémy s onboarding stroje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141660"
---
# <a name="issues-with-onboarding-machines"></a>Problémy s onboarding stroje

Môžete mať problémy s onboarding stroje mdatp služby. Ak máte prístup k počítaču koncového používateľa, postupujte nasledovne:

1. Prevezmite diagnostický nástroj [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)
2. Extrahujte a spustite MDATPAnalyzer.cmd.
3. Vyhľadajte diagnostický denník v priečinku s názvom MDATPClientAnalyzerResult, rovnaký priečinok, kde je prevzatý nástroj Analyzer.
4. Skontrolujte súbor denníka, MDATPClientAnalyzer.txt, nájsť problémy s nastavením pripojenia alebo internetového servera proxy.