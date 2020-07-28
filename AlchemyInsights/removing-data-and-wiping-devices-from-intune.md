---
title: Odstránenie údajov a utieranie zariadení z intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440467"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odstránenie údajov a utieranie zariadení z intune

Vzdialené akcie Zariadenia v režime odchodu do dôchodku a Vymazanie zariadení možno použiť na odstránenie údajov spoločnosti spravovaných spoločnosťou Intune alebo na obnovenie výrobných nastavení a vrátenie zariadenia do predvolených nastavení.

1. Prihláste sa do služby Správa zariadení od spoločnosti Microsoft 365 a prejdite do ponuky **Devices**  >  **All Devices (Všetky zariadenia).**
2. Vyberte zariadenie, ktoré chcete vymazať.
3. Vyberte typ vzdialeného vymazania, ktoré chcete urobiť. Odchod do dôchodku odstráni iba organizačné informácie, zatiaľ čo úplné vymazanie obnoví výrobné nastavenia zariadenia.
4. Výber **potvrďte výberom** položky Yes (Áno). Kým vymazanie skončí, stav akcie zariadenie sa zobrazí ako Odchod do dôchodku čakajúce.</br>
    Po dokončení akcie sa mobilné zariadenie už nebude nachádzať v zozname spravovaných zariadení.

**Upozornenie:** Údaje spoločnosti nie je možné odstrániť zo zariadení pripojených k službe Azure AD.

Podrobné informácie o účinku akcií Odísť do dôchodku a Vymazanie vrátane toho, čo sa zachová a čo sa odstráni, nájdete [v téme Odstránenie zariadení pomocou vymazania, odchodu do dôchodku alebo manuálneho zrušenia zariadenia](https://docs.microsoft.com/intune/devices-wipe).

Ak chcete vymazať všetky údaje zo zariadenia so systémom macOS, pozrite [si tému Vymazanie všetkých údajov zo zariadenia so systémom macOS](https://docs.microsoft.com/intune/device-erase).