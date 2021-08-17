---
title: Nástroj na diagnostiku služby pre Windows virtuálnu pracovnú plochu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052401"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Nástroj na diagnostiku služby pre Windows virtuálnu pracovnú plochu

Windows Virtual Desktop (WVD) ponúka diagnostický nástroj, ktorý umožňuje správcom identifikovať chyby prostredníctvom jedného rozhrania. Tento nástroj zaznamenáva diagnostické informácie vždy, keď WVD použije niekto s priradenou rolou WVD. Každý denník obsahuje informácie o role WVD, ktorá je súčasťou aktivity, chybových hláseniach, ktoré sa zobrazujú počas relácie, a informácie o nájomníkovi a používateľovi. Analýzu denníka služby Azure je možné nakonfigurovať na zaznamenávanie denníka aktivít vytvoreného diagnostickým nástrojom. Postupujte takto:

1. Vytvorte pracovný priestor analýzy denníka pomocou portálu [Azure alebo](https://go.microsoft.com/fwlink/?linkid=2129500) prostredia [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Pripojenie Windows počítačov na Monitor Azure.](https://go.microsoft.com/fwlink/?linkid=2129913) Získajte ID pracovného priestoru a hlavný kľúč pracovného priestoru. Sprievodca nastavením potrebuje tieto informácie, aby správne nakonfiguroval agenta a zaistil, že bude komunikovať so službou Azure Monitor.
1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Diagnostické údaje môžete z nájomníka WVD tlačiť do analýzy denníka svojho pracovného priestoru.
1. [Identifikujte a diagnostikujte](https://go.microsoft.com/fwlink/?linkid=2128338) problémy, ktoré sú vo vzťahu k WVD interné alebo externé.

Ďalšie informácie o konfigurácii diagnostického nástroja služby pre WVD nájdete v téme [Použitie analýzy denníka pre diagnostické funkcie.](https://go.microsoft.com/fwlink/?linkid=2128084)
