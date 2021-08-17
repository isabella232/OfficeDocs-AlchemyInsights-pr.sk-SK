---
title: rovnaké ako je najlepšie názov súboru
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
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312840"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Požadovaná hlavička Alchemy H1, H2 nefunguje."
Osvedčené postupy a pokyny na vytváranie v spoločnosti Alchemy:

1. **Vnoriť do priečinkov Prehľady služby Alchemy**– týmto sa preruší štruktúra URL adresy. Pracujeme na oprave tohto problému.
1. Súbory v priečinku **AlchemyInsights by** mali mať malé názvy súborov so spojovníkmi pre medzery, napríklad. **_how-to-enable-litigation-hold._**
    1. Do poľa ms.custom zahreňte ID pravidla alebo identifikátor sektora z portálu spoločnosti [Alchemy Partner portal.](https://alchemyportal.azurewebsites.net) Napríklad ***ms.custom: 100021***
1. Ako šablónu použite zvyšné metaúdaje v hornej časti tohto súboru.
1. Na [portáli partnera služby Alchemy](https://alchemyportal.azurewebsites.net)prejdite nadol na časť Názov prehľadu **zákazníkov:** a použite ju ako východiskový bod pre názov H1 pre prehľad. 

**Poznámka:** Prehľady Alchemy musí mať v hornej časti len jeden H1, inak sa preruší ich výroba. H2s nevykresľujú ani také, že na **označenie** samostatných sekcií použite tučné písmo alebo iné konvencie.
1. Ďalej vyplňte základný text pomocou konceptového materiálu do časti Customer Insights stránky pravidla služby Alchemy.
    1. Zoznamy s odrážkami sú v poriadku
    1. Číslované zoznamy
    1. **Tučné** písmo a *kurzíva* sú v poriadku
    1. Prepojenia by mali vždy byť **"prepojenia na web"/externé** alebo priame prepojenia na **prvky používateľského rozhrania**, nie na interné prepojenia.
    1. Obrázky v tejto dobe oficiálne nie sú podporované, ale sú v pláne.

Je to už veľmi dlho. Osvedčený postup je približne 400 ---------------------------------

Keď bude obsah pripravený, potiahnite ho do živej vetvy. Potom prejdite na portál [partnera služby Alchemy a](https://alchemyportal.azurewebsites.net) zadajte názov súboru do poľa URL adresy. 