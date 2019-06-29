---
title: Pomocou nástroja nasadenia Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365540"
---
# <a name="using-the-office-deployment-tool-odt"></a>Pomocou Office Deployment Tool (ODT)

Nasadiť Office 365 verzie balíka Office pomocou Office Deployment Tool (ODT). Office Deployment Tool (setup.exe) je spustiť z príkazového riadka a používa konfiguračný XML súbor zistiť, aké nastavenia použiť pri nasadzovaní balíka Office.
  
1. Stiahnite si najnovšiu verziu nástroja nasadenia Office z [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Použite [Nástroj na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorenie konfiguračného XML súboru. Export konfiguračný súbor a umiestnite ho lokálne v rovnakom priečinku kde býva setup.exe.

    **Poznámka:** Inštaláciu balíka Office bežne vyskytnúť problémy vzhľadom na zle alebo malformatted konfiguračné súbory. Aby sa predišlo také problémy, odporúčame, že používate nástroj na prispôsobenie balíka Office vytvoriť konfiguračný súbor. Môžete tiež importovať existujúce konfiguračné súbory do nástroj na prispôsobenie balíka Office.

3. Z námer kontrolovať vrtký, prepnite do polohy bydliska setup.exe a spustite nástroj na nasadenie balíka Office v režime stiahnutie a určite konfiguračný súbor ste práve uložili. V tomto príklade, konfiguračný súbor sa nazýva Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Spustenie nástroja nasadenia Office v Konfigurácia režimu a zadajte konfiguračný súbor.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Poznámka:** Tento krok musíte spustiť z klientskeho počítača, na ktorom chcete nainštalovať balík Office a musíte mať povolenia lokálneho správcu na tomto počítači.

Ďalšie informácie o používaní nástroja nasadenia Office pre Office 365 ProPlus scenáre nasadenia, pozrite si [Prehľad nástroja nasadenia Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Pre viac informácií o tom, ako používať nástroj na prispôsobenie balíka Office, nájdete v časti [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
