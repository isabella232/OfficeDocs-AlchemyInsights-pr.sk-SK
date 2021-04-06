---
title: Diagnostický nástroj služby pre virtuálnu pracovnú plochu Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596041"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Diagnostický nástroj služby pre virtuálnu pracovnú plochu Windowsu

Windows Virtual Desktop (WVD) ponúka diagnostický nástroj, ktorý umožňuje správcom identifikovať chyby prostredníctvom jedného rozhrania. Tento nástroj zaznamenáva diagnostické informácie vždy, keď WVD použije niekto s priradenou rolou WVD. Každý denník obsahuje informácie o role WVD, ktorá je súčasťou aktivity, chybových hláseniach, ktoré sa zobrazujú počas relácie, a informácie o nájomníkovi a používateľovi. Analýzu denníka služby Azure je možné nakonfigurovať na zaznamenávanie denníka aktivít vytvoreného diagnostickým nástrojom pomocou týchto krokov:

1. Vytvorte pracovný priestor analýzy denníka pomocou portálu [Azure alebo](https://go.microsoft.com/fwlink/?linkid=2129500) prostredia [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Pripojte počítače s Windowsom k monitoru Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Získajte ID pracovného priestoru a hlavný kľúč pracovného priestoru. Sprievodca nastavením potrebuje tieto informácie, aby správne nakonfiguroval agenta a zaistil, že bude komunikovať so službou Azure Monitor.

1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Diagnostické údaje môžete z nájomníka WVD tlačiť do analýzy denníka svojho pracovného priestoru.

1. [Identifikujte a diagnostikujte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problémy, ktoré sú vo vzťahu k WVD interné alebo externé.

Ďalšie informácie o konfigurácii diagnostického nástroja služby pre WVD nájdete v téme Použitie analýzy denníka pre diagnostické funkcie.