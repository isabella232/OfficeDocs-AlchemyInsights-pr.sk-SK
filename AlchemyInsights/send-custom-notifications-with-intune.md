---
title: Odoslanie vlastných oznámení so službou Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720661"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Odoslanie vlastných oznámení používateľom spravovaných zariadení so systémom iOS a Android

Vlastné oznámenia pre služby Intune sú spracované v aplikácii Company Portal v zariadení používateľa. Aplikácia potom vytvorí oznámenie o vyžiadaní v danom zariadení.

Nižšie sú uvedené požiadavky zariadenia, ktoré podporujú prijímanie vlastných oznámení, a v aplikácii potom vytvorte Push Oznámenie:

- Zariadenie musí mať nainštalovanú aplikáciu firemný portál.  

- Zariadenie musí povoliť, aby aplikácia spoločnosti Portal odoslala oznámenia push. Pri inštalácii alebo aktualizácii aplikácie sa používateľovi zobrazí výzva na povolenie oznámení.

- Zariadenia s Androidom musia mať nainštalované služby Google Play.

- Zariadenie musí byť zaregistrované v službe Intune.

Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkciám](https://docs.microsoft.com/intune/custom-notifications).
