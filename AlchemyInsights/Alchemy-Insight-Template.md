---
title: rovnako ako názov súboru je najvhodnejší
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664149"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Požadovaná alchýmia header H1, H2's nefungujú."
Najvhodnejšie postupy a pokyny na vytváranie alchýmie:

1. Do **not Nest alchýmia prehľady v priečinkoch**– tým sa preruší štruktúra URL adresy. My sme hľadali riešenie tohto.
1. Súbory v priečinku **AlchemyInsights** by mali obsahovať malé názvy súborov s pomlčkami pre medzery ex. ***postup – povolenie – zadržanie***.
    1. Zahrňte ID pravidla alebo identifikáciu vedierko z [partnerského portálu alchýmie](https://alchemyportal.azurewebsites.net) do poľa MS. custom. napríklad. ***MS. Custom: 100021***
1. Použite zvyšok metaúdajov v hornej časti tohto súboru ako šablónu.
1. Na [partnerskom portáli alchýmie](https://alchemyportal.azurewebsites.net)prejdite nadol na časť **názov prehľadu zákazníka:** a použite ho ako východiskový bod pre názov H1 pre prehľad. 
    > [!NOTE]
    > Podrobné informácie o alchýmii musia mať v hornej časti iba jeden H1 alebo sa rozkladajú vo výrobe. H2s Nekresliť ani tak použite **tučné písmo** alebo iné konvencie označujúce samostatné sekcie.
1. Potom vyplňte základný text pomocou konceptu materiál v časti prehľady zákazníkov na stránke pravidiel alchýmie.
    1. Zoznamy s odrážkami sú v pohodě
    1. Číslované zoznamy
    1. **Tučné písmo** a *kurzíva* sú a-OK
    1. Prepojenia by mali byť vždy buď **"prepojenia na web"/external** alebo **hlboké prepojenia na prvky používateľského rozhrania**, nie interné prepojenia.
    1. Obrázky nie sú v súčasnosti oficiálne podporované, ale je to na pláne.

A to je naozaj už trochu príliš dlho. Najvhodnejšie postupy sú približne 400 znakov---------------------------------

Keď je váš obsah pripravený, presuňte ho do živej vetvy. Potom prejdite na [partnerský portál alchýmie](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa URL adresa. 