---
title: Odosielanie vlastných upozornení pomocou Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992327"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Ako posielať vlastné oznámenia používateľom spravovaných iOS a Android zariadenia

Vlastné upozornenia pre Intune spracováva aplikácia portálu spoločnosti v zariadení používateľa. Aplikácia potom vytvorí oznámenie push na tomto zariadení.

Nižšie sú uvedené predpoklady zariadenia na podporu prijímania vlastných upozornení a pre aplikáciu na vytvorenie oznámenia push:

- Zariadenie musí mať nainštalovanú aplikáciu portálu spoločnosti.  

- Zariadenie musí povoliť aplikácii portálu spoločnosti odosielať oznámenia push. Keď je aplikácia nainštalovaná alebo aktualizovaná, vyzve používateľa na povolenie upozornení.

- Zariadenia so systémom Android musia mať nainštalované služby Google Play.

- Zariadenie musí byť zapísané s Intune.

Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkcii](https://docs.microsoft.com/intune/custom-notifications).
