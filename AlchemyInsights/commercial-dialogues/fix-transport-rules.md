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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750575"
---
# <a name="fix-transport-rules"></a>Oprava pravidiel prenosu

Táto správa ovplyvnila vlastné pravidlo toku pošty. Ak chcete skontrolovať presné pravidlo, postupujte takto:

1. Vo výsledkoch odosielania v časti **Ďalšie informácie** si všimnite **identifikátor GUID** alebo **názov politiky**.
2. Spustite prostredie Exchange Management Shell. Ďalšie informácie nájdete v téme [Otvorenie prostredia Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Spustite tento príkaz (pomocou identifikátora GUID z vášho odoslania):  **Get-TransportRule-identity "GUID" | FL * Popis***
4. Prezrite si popis a zobrazia sa nakonfigurované podmienky, ktoré ovplyvnili správu.

Ďalšie informácie nájdete v téme [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
