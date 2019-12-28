---
title: Odosielanie vlastných upozornení pomocou Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886872"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Ako posielať vlastné oznámenia používateľom spravovaných iOS a Android zariadenia

Vlastné upozornenia pre Intune spracováva aplikácia portálu spoločnosti v zariadení používateľa. Aplikácia potom vytvorí oznámenie push na tomto zariadení.

Nižšie sú uvedené predpoklady zariadenia na podporu prijímania vlastných upozornení a pre aplikáciu na vytvorenie oznámenia push:

- Zariadenie musí mať nainštalovanú aplikáciu portálu spoločnosti.  

- Zariadenie musí povoliť aplikácii portálu spoločnosti odosielať oznámenia push. Keď je aplikácia nainštalovaná alebo aktualizovaná, vyzve používateľa na povolenie upozornení.

- Zariadenia so systémom Android musia mať nainštalované služby Google Play.

- Zariadenie musí byť zapísané s Intune.

Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkcii](https://docs.microsoft.com/intune/custom-notifications).
