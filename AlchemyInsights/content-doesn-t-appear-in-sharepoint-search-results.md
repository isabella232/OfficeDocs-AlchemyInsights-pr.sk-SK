---
title: Obsah sa nezobrazuje vo výsledkoch vyhľadávania v SharePointe
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713145"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Obsah sa nezobrazuje vo výsledkoch vyhľadávania v SharePointe

Postupujte podľa týchto krokov na riešenie problémov, keď sa očakávaný obsah vo výsledkoch vyhľadávania nezobrazuje:
  
1. Skontrolujte, či je **lokalita** , ktorá obsahuje očakávaný obsah, nastavená tak, aby umožňovala zobrazovanie obsahu vo výsledkoch vyhľadávania. Postupujte podľa krokov v téme [zobrazenie obsahu na lokalite vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Skontrolujte, či je **zoznam** alebo **knižnica** , ktorá obsahuje očakávaný obsah, nastavená na možnosť Zobraziť obsah vo výsledkoch vyhľadávania. Postupujte podľa krokov v téme [zobrazenie obsahu zo zoznamov alebo knižníc vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Overte, či je stránka, dokument alebo vlastné rozloženie strany publikovaná ako **hlavná verzia.** Sledovať krok 3 vo [vyhľadávaní nevráti všetky výsledky v SharePointe Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Overte, či má používateľ **povolenia** na zobrazenie obsahu. Postupujte podľa krokov uvedených v téme [úrovne povolení v SharePointe](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ak sa schéma vyhľadávania zmenila pridaním novej spravovanej vlastnosti úpravou spravovanej vlastnosti alebo odstránením spravovanej vlastnosti, bude sa požadovať požadovanie prehľadávania obsahu a opätovného indexu. **Opätovné indexovanie** obsahu podľa krokov uvedených v téme [manuálne vyžiadanie prehľadávania obsahu a opätovného indexovania lokality, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-content). Môže to chvíľu trvať, počkajte 24 hodín, kým znova nebudete kontrolovať výsledky.

Ďalšie informácie nájdete v téme [povolenie vyhľadávania obsahu na lokalite](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
