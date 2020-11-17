---
title: Používanie nástroja na nasadenie balíka Office
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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085847"
---
# <a name="using-the-office-deployment-tool-odt"></a>Použitie nástroja na nasadenie balíka Office (ODT)

Pomocou nástroja na nasadenie balíka Office (ODT) môžete nasadiť verzie balíka Office 365. Nástroj na nasadenie balíka Office (setupodt.exe) sa spustí z príkazového riadkov a použije súbor konfigurácie XML na určenie nastavení, ktoré sa majú použiť pri nasadení balíka Office.
  
1. Stiahnite si najnovšiu verziu nástroja na nasadenie balíka Office z [Centra sťahovania](https://go.microsoft.com/fwlink/p/?LinkID=626065)softvéru.

2. Pomocou [nástroja na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorte súbor XML konfigurácie. Exportujte konfiguračný súbor a umiestnite ho lokálne do rovnakého priečinka, v ktorom sa nachádza setupodt.exe.

    **Poznámka:** Problémy s inštaláciou balíka Office sa bežne vyskytujú v dôsledku nesprávne konfigurovaných alebo malformatted konfiguračných súborov. Ak sa chcete vyhnúť takýmto problémom, odporúčame, aby ste na vytvorenie konfiguračného súboru použili nástroj na prispôsobenie balíka Office. Existujúce konfiguračné súbory môžete importovať aj do nástroja na prispôsobenie balíka Office.

3. V príkazovom riadku s právami správcu prejdite na miesto, kde sa setupodt.exe nachádza, a spustite nástroj na nasadenie balíka Office v režime sťahovania a zadajte konfiguračný súbor, ktorý ste práve uložili. V tomto príklade sa konfiguračný súbor nazýva Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Spustite nástroj na nasadenie balíka Office v režime konfigurácie a zadajte konfiguračný súbor.

```setupodt.exe /configure Configuration.xml```

**Poznámka:** Tento krok musíte spustiť z klientskeho počítača, v ktorom chcete nainštalovať balík Office, a musíte mať v danom počítači povolenia lokálneho správcu.

Ďalšie informácie o používaní nástroja na nasadenie balíka Office pre aplikácie Microsoft 365 pre scenáre podnikového nasadenia nájdete v téme [Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Ďalšie informácie o používaní nástroja na prispôsobenie balíka Office nájdete v téme [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
