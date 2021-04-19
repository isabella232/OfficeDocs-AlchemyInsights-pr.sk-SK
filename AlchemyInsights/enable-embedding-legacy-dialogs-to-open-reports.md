---
title: Povolenie vkladania starších dialógových okna na otváranie zostáv
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814279"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Povolenie vkladania starších dialógových okna na otváranie zostáv

**Príznak**

Používatelia nemôžu otvárať zostavy. Niečo sa pokazilo. Check technical details for more details".

**Príčina**

Zostavy zlyhávajú pri načítaní v UCI s chybou " Popisovač formulára je null alebo nie je definovaný." Zostavy v UCI stále vyžadujú staršie dialógové okná, takže systém zákazníka musí mať povolené povolenie *delegovaniadialogsembe u zákazníkov.*

**Riešenie**

1. Prejdite na **položky >Správa > kartu Nastavenie > Všeobecné**.

2. Nastavte položku Povoliť vkladanie niektorých starších dialógových oknách v klientovi prehliadača so zjednotením rozhrania na možnosť **Áno.**
