---
title: Najlepšie je rovnaký ako názov súboru
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742458"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Vyžaduje alchýmie hlavičke H1, H2-nefungujú.
Najlepšie postupy a pokyny pre authoring alchýmia:

1. **Nest alchýmia postrehy v priečinkoch**- to bude prestávka v url štruktúru. Hľadáme do stanovenie tejto.
1. Súbory v priečinku **AlchemyInsights** by mali mať malé písmená názvov súborov s pomlčkami medzery ex. ***jak-na-enable--zadržanie***.
    1. Zahŕňajú identifikácia pravidla alebo vedierko ID z [alchýmie Partner portal](https://alchemyportal.azurewebsites.net) v poli ms.custom. ex. ***MS.Custom: 100021***
1. Použite zvyšok metaúdaje v hornej časti tohto súboru ako šablóny.
1. [Alchýmia Partner portal](https://alchemyportal.azurewebsites.net)prejdite nadol do sekcie **zákazníka Insight titul:** a použiť ho ako východiskový bod pre nadpis H1 pre pochopenie. 
    > [!NOTE]
    > Alchýmia poznatky musí mať iba jeden H1 navrchu alebo bude prestávka vo výrobe. H2s neznemožňujú tak použiť **tučné** alebo iných dohovorov znamenať samostatných sekcií.
1. Ďalšie, vyplňte základný text pomocou návrh materiálu v časti prehľady o zákazníkoch alchýmia pravidlo stránky
    1. Zoznamy s odrážkami sú v poriadku
    1. Číslované zoznamy príliš
    1. **Tučné písmo** a *kurzíva* sú a-ok
    1. Odkazy by mali byť vždy buď **"Odkazy na web" / externý** alebo **hlboko-odkazy na prvky používateľského rozhrania**, nie interné odkazy.
    1. Obrázky nie sú oficiálne podporované v tejto dobe, ale to je na pláne.

A to je naozaj už trochu príliš dlho. Najlepšie je asi 400 znakov---

Akonáhle váš obsah je pripravený, vytiahnite ju na živé vetvy. Potom [alchýmia Partner portálu](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url. M