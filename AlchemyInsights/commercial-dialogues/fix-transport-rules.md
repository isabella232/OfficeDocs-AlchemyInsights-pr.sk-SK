---
title: Oprava pravidiel prenosu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034769"
---
# <a name="fix-transport-rules"></a>Oprava pravidiel prenosu

Toto pravidlo toku pošty ovplyvnilo toto pravidlo. Ak chcete skontrolovať presné pravidlo, vykonajte nasledovné kroky:

1. Vo výsledkoch odoslania si v časti **Ďalšie informácie** poznačte **identifikátor GUID** alebo **názov politiky.**
2. Spustite Exchange Management Shell. Ďalšie informácie nájdete v téme [Otvorenie Exchange správy e-Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Spustite tento príkaz (pomocou identifikátora GUID z príspevku):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Ak chcete zobraziť konfigurované podmienky, ktoré ovplyvnili hlásenie, prečítajte si popis.

Ďalšie informácie nájdete v téme [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
