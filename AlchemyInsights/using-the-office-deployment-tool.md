---
title: Pomocou nástroja Office Deployment
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010885"
---
# <a name="using-the-office-deployment-tool-odt"></a>Používanie nástroja na nasadenie balíka Office (ODT)

Používate Office Deployment Tool (ODT) nasadiť Office 365 verzie balíka Office. Nástroj na nasadenie balíka Office (Setup. exe) je spustený z príkazového riadka a používa konfiguračný súbor XML na určenie nastavení, ktoré sa použijú pri nasadzovaní balíka Office.
  
1. Prevezmite najnovšiu verziu nástroja na nasadenie balíka Office z [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomocou [nástroja na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorte súbor XML konfigurácie. Exportujte konfiguračný súbor a umiestnite ho lokálne na rovnaký priečinok, kde sa nachádza Setup. exe.

    **Poznámka:** Problémy s inštaláciou balíka Office sa bežne vyskytujú v dôsledku chybne nakonfigurovaných alebo chybne formátovaných konfiguračných súborov. Aby sa predišlo takýmto problémom, odporúčame použiť nástroj na prispôsobenie balíka Office vytvoriť konfiguračný súbor. Môžete tiež importovať existujúce konfiguračné súbory do nástroja na prispôsobenie balíka Office.

3. Z príkazového riadka s právami správcu prepnite do umiestnenia, kde sa nachádza súbor Setup. exe, a spustite nástroj na nasadenie balíka Office v režime preberania a zadajte konfiguračného súboru, ktorý ste práve uložili. V tomto príklade konfiguračný súbor s názvom Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Spustite nástroj Office Deployment v režime konfigurovať a zadajte konfiguračný súbor.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Poznámka:** Tento krok musíte spustiť z klientskeho počítača, na ktorom chcete nainštalovať balík Office a musíte mať povolenia lokálneho správcu na danom počítači.

Ďalšie informácie o používaní nástroja na nasadenie balíka Office pre Microsoft 365 aplikácie pre podnikové nasadenie scenáre, pozrite si [Prehľad nástroja Office Deployment](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Ďalšie informácie o používaní nástroja na prispôsobenie balíka Office nájdete v téme [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
