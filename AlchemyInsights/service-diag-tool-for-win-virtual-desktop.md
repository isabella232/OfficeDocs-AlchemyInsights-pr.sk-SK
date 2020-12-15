---
title: Nástroj na diagnostiku služby pre virtuálnu pracovnú plochu Windowsu
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680231"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Nástroj na diagnostiku služby pre virtuálnu pracovnú plochu Windowsu

Windows Virtual Desktop (WVD) ponúka diagnostický nástroj, ktorý umožňuje správcom identifikovať chyby prostredníctvom jedného rozhrania. Tento nástroj zapisuje informácie súvisiace s diagnostikou pri každom použití WVD používateľom priradenej roly WVD. Každý denník obsahuje informácie o WVD úlohe zahrnutej v aktivite, chybových správach, ktoré sa zobrazujú počas relácie, a informácie o nájomníkovi a používateľovi. Analýzu denníka služby Azure je možné nakonfigurovať tak, aby zaznamenávala denník aktivít vytvorený diagnostickým nástrojom. Postupujte takto:

1. Vytvorenie pracovného priestoru denníka analýzy pomocou [portálu Azure](https://go.microsoft.com/fwlink/?linkid=2129500) alebo [prostredia Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Pripojte počítače s Windowsom k službe Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Získajte identifikáciu pracovného priestoru a hlavný kľúč pracovného priestoru. Sprievodca nastavením vyžaduje, aby tieto informácie správne nakonfigurovali agenta a zaistili, že dokážu komunikovať so službou Azure monitor.
1. [Vytlačte údaje diagnostiky do pracovného priestoru](https://go.microsoft.com/fwlink/?linkid=2128284). Údaje o diagnostike môžete tlačiť z nájomníka WVD do denníka Analytics pre váš pracovný priestor.
1. [Identifikujte a diagnostikujte problémy](https://go.microsoft.com/fwlink/?linkid=2128338) , ktoré sú interné alebo externé vo vzťahu k WVD.

Ďalšie informácie o konfigurácii nástroja Diagnostika služby pre WVD nájdete v téme [použitie funkcie Denníková analýza pre funkciu diagnostiky](https://go.microsoft.com/fwlink/?linkid=2128084).
