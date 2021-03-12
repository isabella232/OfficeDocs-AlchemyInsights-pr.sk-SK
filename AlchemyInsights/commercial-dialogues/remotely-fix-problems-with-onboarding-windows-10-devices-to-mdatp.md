---
title: Riešenie problémov s integrovaním zariadení s Windowsom 10 do rozšírenej ochrany pred hrozbami programu Microsoft Defender na diaľku
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750042"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Riešenie problémov s integrovaním zariadení s Windowsom 10 do rozšírenej ochrany pred hrozbami programu Microsoft Defender na diaľku

Ak máte prístup k vzdialenému počítaču, postupujte podľa týchto krokov:

1. Stiahnite si diagnostický nástroj [analyzátor pripojenia klienta](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Extrahujte a spustite MDATPAnalyzer. cmd.
3. Vyhľadajte diagnostický denník v priečinku MDATPClientAnalyzerResult, ktorý sa nachádza v tom istom priečinku, v ktorom bol nástroj analyzátor stiahnutý.
4. Ak chcete nájsť problémy s pripojením alebo nastavením internetového servera proxy, skontrolujte súbor denníka MDATPClientAnalyzer.txt.

Ďalšie informácie nájdete v téme [problémy s integrovanými strojmi](https://go.microsoft.com/fwlink/?linkid=2143634).
