---
title: 'rovnaký ako názov súboru je najlepšie [pravidlo #-Popis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697145"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Vyžaduje alchýmie hlavičke H1, H2-nefungujú.
Najlepšie postupy a pokyny pre authoring alchýmia:

1. **Nest alchýmia postrehy v priečinkoch**- to bude prestávka v url štruktúru. Hľadáme do stanovenie tejto.
1. Súbory v priečinku **AlchemyInsights** by mali mať identifikácia pravidla a pravidlo názov z [alchýmie Partner portálu](https://alchemyportal.azurewebsites.net) v názve súboru.
    1. ex. ***976-How-to-enable-litigation-hold***
1. Metadáta použiť v hornej časti tento súbor ako šablónu. Nič iné nevyžaduje.
1. [Alchýmia Partner portal](https://alchemyportal.azurewebsites.net)prejdite nadol do sekcie **zákazníka Insight titul:** a použiť ho ako východiskový bod pre nadpis H1 pre pochopenie. 
    > [!NOTE]
    > Alchýmia poznatky musí mať iba jeden H1 navrchu alebo bude prestávka vo výrobe. H2s neznemožňujú tak použiť **tučné** alebo iných dohovorov znamenať samostatných sekcií.
1. Ďalšie, vyplňte základný text pomocou návrh materiálu v časti prehľady o zákazníkoch alchýmia pravidlo stránky
    1. Zoznamy s odrážkami sú v poriadku
    1. Číslované zoznamy príliš
    1. **Tučné písmo** a *kurzíva* sú a-ok
    1. Odkazy by mali byť vždy buď **"Odkazy na web" / externý** alebo **hlboko-odkazy na prvky používateľského rozhrania**, nie interné odkazy.

A to je naozaj už trochu príliš dlho. Najlepšie je asi 400 znakov---

Akonáhle váš obsah je pripravený, vytiahnite ju na živé vetvy. Potom [alchýmia Partner portálu](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url. Uistite sa, že pohľad Review a publikovanej hovorí "áno" a kliknite na tlačidlo pravidlo pre aktualizáciu. **(To bude vyzerať hezčí v novej verzii portálu - uvoľnenie čoskoro.)** 
 ![url poľa](media/for-content-team.PNG)

