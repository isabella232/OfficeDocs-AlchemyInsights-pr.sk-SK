---
title: Prevod poštovej schránky používateľa do zdieľanej poštovej schránky?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906747"
---
Poštovú schránku môžete preniesť len k zdieľanej schránke Ak používateľ nemá licenciu Exchange. Po skonvertovaní poštovej schránky sa bude naďalej zobrazovať v zozname aktívnych užívateľov, pretože tento zoznam obsahuje zdieľané poštové schránky. Však prevedený poštovej schránky sa tiež zobrazí v zozname zdieľanej poštovej schránky. 
  
Ak sa pokúsite previesť poštovej schránky Exchange Admin konzoly a prevod zlyhá, vymažte vyrovnávaciu pamäť prehliadača a súbory cookie a skúste znova. Ak to stále nefunguje, skúste prevod poštovej schránky v prostredí Exchange Management Shell spustením nasledujúceho príkazu:
  
```
Set-Mailbox -Type Shared
```

Viac konverzií informácie poštovej schránky je k dispozícii v [prevod používateľa poštovej schránky zdieľanej poštovej schránke](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
