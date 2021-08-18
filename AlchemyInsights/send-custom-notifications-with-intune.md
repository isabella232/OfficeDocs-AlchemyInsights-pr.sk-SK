---
title: Odosielanie vlastných oznámení pomocou intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086179"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Postup odosielania vlastných oznámení používateľom spravovaných zariadení so systémom iOS a Android

Vlastné oznámenia pre Intune spracováva aplikácia Company Portal v zariadení používateľa. Aplikácia potom v tomto zariadení vytvorí oznámenie bez upozornenia.

Nasledujúce požiadavky sú nevyhnutnými predpokladmi na podporu potvrdení o vlastných oznámeniach a na to, aby aplikácia potom vytvorila oznámenie bez oznámenia:

- Zariadenie musí mať nainštalovanú Company Portal aplikáciu.  

- Zariadenie musí povoliť aplikácii Company Portal odosielať oznámenia bez oznámenia. Po nainštalovaní alebo aktualizovaní aplikácie sa používateľovi zobrazí výzva na povolenie oznámení.

- Zariadenia s Androidom musia mať nainštalované služby Google Play.

- Zariadenie musí byť zaregistrované v intune.

Ďalšie informácie vrátane informácií o tom, ako odoslať správu, nájdete v [dokumentácii k funkcii.](https://docs.microsoft.com/intune/custom-notifications)
