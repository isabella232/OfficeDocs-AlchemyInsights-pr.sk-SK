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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003404"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Povolenie vkladania starších dialógových okna na otváranie zostáv

**Príznak**

Používatelia nemôžu otvárať zostavy. Niečo sa pokazilo. Check technical details for more details".

**Príčina**

Zostavy zlyhávajú pri načítaní v UCI s chybou " Popisovač formulára je null alebo nie je definovaný." Zostavy v UCI stále vyžadujú staršie dialógové okná, takže systém zákazníka musí mať povolené povolenie *delegovaniadialogsembe u zákazníkov.*

**Riešenie**

1. Prejdite na **Nastavenia >na > systém Nastavenia > všeobecné.**

2. Nastavte položku Povoliť vkladanie niektorých starších dialógových oknách v klientovi prehliadača so zjednotením rozhrania na možnosť **Áno.**
