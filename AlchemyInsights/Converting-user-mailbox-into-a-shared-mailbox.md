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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496450"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konvertovať zdieľanú poštovú schránku používateľa e-mailovej schránky

Poštovú schránku môžete preniesť len k zdieľanej schránke Ak používateľ nemá licenciu Exchange. Po skonvertovaní poštovej schránky sa bude naďalej zobrazovať v zozname aktívnych užívateľov, pretože tento zoznam obsahuje zdieľané poštové schránky. Však prevedený poštovej schránky sa tiež zobrazí v zozname zdieľanej poštovej schránky. 
  
Ak sa pokúsite previesť poštovej schránky Exchange Admin konzoly a prevod zlyhá, vymažte vyrovnávaciu pamäť prehliadača a súbory cookie a skúste znova. Ak to stále nefunguje, skúste prevod poštovej schránky v prostredí Exchange Management Shell spustením nasledujúceho príkazu:
  
```
Set-Mailbox -Type Shared
```

Viac konverzií informácie poštovej schránky je k dispozícii v [prevod používateľa poštovej schránky zdieľanej poštovej schránke](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
