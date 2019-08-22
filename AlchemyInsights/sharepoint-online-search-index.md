---
title: Vyhľadávanie v službe SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507646"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Prehľadávanie obsahu a indexovanie v SharePoint Online

Obsah musí prechádzať a pridali do vyhľadávacieho indexu užívateľom nájsť, čo hľadajú v SharePoint Online. Automaticky prehľadávania obsahu založené na vopred definovaných crawl plán (plán prehľadávania obsahu nie je možné zmeniť). Modul na prehľadávanie obsahu sa zdvihne obsah, ktorý sa zmenil od posledného prehľadávania a aktualizuje register. Na zabezpečenie prehľadávania obsahu a aktualizácia registra prebieha, uvedomte si nasledovné:

- Uistite sa, že obsah možno nájsť tým, [že obsah stránky vyhľadávať](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Keď ste zmenili spravovanú vlastnosť, alebo keď ste zmenili mapovanie liezol a spravované vlastnosti, stránky musí byť opätovne prehľadaný pred zmeny sa prenesú do indexu vyhľadávania. 

    Pretože vaše zmeny v schéme Hľadať, a nie skutočné stránky, crawler nebude automaticky znovu index stránky. 

    Ďalšie informácie nájdete v téme [manuálne požiadať o plazenie a opätovné indexovanie stránky, knižnice alebo zoznamu](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Počkajte aspoň 24 hodín po manuálne požiadať plaziť a plné re-index vidieť, ak máte stále problém. 

    Ak od uskutočnenia prehľadávania obsahu a plnej preindexovania spracoval uplynulo viac ako 24 hodín, prihláste sa podpory prípadu. V mnohých prípadoch už pracujeme na riešení. Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.

> [!IMPORTANT]
> Ak lokalitu, dokument (Knižnica) alebo zoznam bol odstránený a stále zobrazuje vo výsledkoch vyhľadávania, používatelia by mali dostávať **Chyba 404 súbor nebol nájdený** pri pokuse o prístup. Tento problém sa zapíšu ako prípad pre ďalšie vyšetrovanie. 



