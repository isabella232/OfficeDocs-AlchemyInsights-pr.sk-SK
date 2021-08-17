---
title: Používanie nástroja Office na nasadenie
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083785"
---
# <a name="using-the-office-deployment-tool-odt"></a>Používanie nástroja Office na nasadenie (ODT)

Pomocou nástroja Office na nasadenie (ODT) môžete nasadiť Office 365 verzií Office. Nástroj Office na nasadenie (setup.exe) sa spúšťa z príkazového riadka a používa konfiguračný súbor XML na určenie toho, aké nastavenia sa majú použiť pri nasadzovaní Office.
  
1. Stiahnite si najnovšiu verziu nástroja na Office na nasadenie z Centra [sťahovania softvéru spoločnosti Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Pomocou nástroja [Office na prispôsobenie (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorte konfiguračný súbor XML. Exportujte konfiguračný súbor a umiestnite ho lokálne do toho istého priečinka, v setup.exe sa nachádza.

    **Poznámka:** Office problémov s inštaláciou sa často vyskytujú z dôvodu nesprávne nakonfigurovaných alebo malformátovaných konfiguračných súborov. Ak sa chcete týmto problémom vyhnúť, odporúčame vám na vytvorenie konfiguračného súboru Office použiť Nástroj na prispôsobenie používateľského prostredia. Môžete tiež importovať existujúce konfiguračné súbory do nástroja Office prispôsobenia.

3. Z príkazového riadka bez oprávnení prepnite na umiestnenie, kde sa setup.exe, a spustite nástroj na nasadenie balíka Office v režime sťahovania a zadajte konfiguračný súbor, ktorý ste práve uložili. V tomto príklade sa konfiguračný súbor nazýva Configuration.xml:

```setup.exe /download Configuration.xml```

4.Spustite nástroj Office na nasadenie v režime konfigurácie a zadajte konfiguračný súbor.

```setup.exe /configure Configuration.xml```

**Poznámka:** Tento krok musíte spustiť z klientskeho počítača, v ktorom chcete nainštalovať Office, a v tomto počítači musíte mať povolenia lokálneho správcu.

Ďalšie informácie o používaní nástroja Office na nasadenie pre scenáre Aplikácie Microsoft 365 pre veľké organizácie nasadenia nájdete v téme Prehľad nástroja [Office na nasadenie](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Ďalšie informácie o používaní Nástroja na prispôsobenie Office nájdete v téme Prehľad nástroja [Office prispôsobenia.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
