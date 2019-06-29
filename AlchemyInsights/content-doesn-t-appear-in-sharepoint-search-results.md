---
title: Obsah sa nezobrazí vo výsledkoch vyhľadávania SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363835"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Obsah sa nezobrazí vo výsledkoch vyhľadávania SharePoint

Postupujte podľa týchto krokov, ak sa nezobrazuje očakávaný obsah vo výsledkoch vyhľadávania:
  
1. Skontrolujte, či **stránka** , ktorá obsahuje očakávaný obsah je nastavený na Povoliť obsah zobrazovať vo výsledkoch vyhľadávania. Postupujte podľa [Zobraziť obsah na mieste vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Skontrolujte, že **zoznam** alebo **knižnicu** , ktorá obsahuje očakávaný obsah je nastavený na Povoliť obsah zobrazovať vo výsledkoch vyhľadávania. Postupujte podľa [Zobraziť obsah zo zoznamov alebo knižníc vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Overiť, že stránky, dokumentu alebo vlastné rozloženie je publikovaná ako **hlavná verzia.** Postupujte podľa kroku 3 v [hľadanie nevrátilo všetky výsledky SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Overte, či má používateľ **povolenia** na zobrazenie obsahu. Postupujte podľa [chápanie úrovní povolení v službe SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Ak schéma vyhľadávania bol zmenený pridaním novú spravovanú vlastnosť, upravovať spravovanú vlastnosť alebo odstránením spravovanú vlastnosť potom žiada plaziť a preindexuje bude vyžadovať. **Opätovné indexovanie** obsahu podľa krokov uvedených v téme [manuálne požiadať o plazenie a opätovné indexovanie stránky, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-content). To môže chvíľu trvať, počkajte 24 hodín pred zisťovaním výsledkov znova.

Ďalšie informácie nájdete v téme [povolenie obsah stránky byť prehľadávateľné](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
