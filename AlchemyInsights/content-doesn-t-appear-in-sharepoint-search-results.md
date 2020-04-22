---
title: Obsah sa nezobrazuje vo výsledkoch vyhľadávania služby SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705676"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Obsah sa nezobrazuje vo výsledkoch vyhľadávania služby SharePoint

Postupujte podľa týchto krokov na riešenie problémov, keď očakávaný obsah nezobrazuje vo výsledkoch vyhľadávania:
  
1. Skontrolujte, či **lokalita** , ktorá obsahuje očakávaný obsah, je nastavená na umožnenie zobrazovania obsahu vo výsledkoch vyhľadávania. Postupujte podľa krokov v zozname [Zobraziť obsah na lokalite vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Skontrolujte, či **zoznam** alebo **knižnica** , ktorá obsahuje očakávaný obsah, je nastavená na povolenie obsahu, ktorý sa má zobraziť vo výsledkoch vyhľadávania. Postupujte podľa krokov v zozname [Zobraziť obsah zo zoznamov alebo knižníc vo výsledkoch vyhľadávania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Overte, či sa stránka, dokument alebo vlastné rozloženie strany publikujú ako **hlavná verzia.** Postupujte krok 3 vo [vyhľadávaní nevráti všetky výsledky SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Overte, či má používateľ **povolenia** na zobrazenie obsahu. Postupujte podľa krokov v [porozumení úrovne povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ak schéma vyhľadávania bola zmenená pridaním novej spravovanej vlastnosti, úpravou spravovanej vlastnosti alebo odstránením spravovanej vlastnosti, požiada sa o prehľadávanie obsahu a opätovný index. **Znova indexovať** obsah podľa krokov v [manuálnej požiadavke prehľadávania a opätovného indexovania lokality, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-content). Môže to chvíľu trvať, počkajte 24 hodín pred opätovným skontrolovaním výsledkov.

Ďalšie informácie nájdete v téme [povolenie vyhľadávania obsahu na lokalite](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
