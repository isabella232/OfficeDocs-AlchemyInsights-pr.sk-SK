---
title: Odstránenie údajov a vymazanie zariadení z Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331056"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odstránenie údajov a vymazanie zariadení z Intune

Vzdialené akcie Vyradenie zariadenia a Vymazanie zariadenia možno použiť na odstránenie podnikových údajov spravovaných službou Intune alebo na resetovanie výrobných nastavení a obnovenie predvolených nastavení zariadenia.

1. Prihláste sa do aplikácie Správa zariadení pre Microsoft 365 a prejdite na položku **Zariadenia** > **Všetky zariadenia**.
2. Vyberte zariadenie, v ktorom chcete údaje vymazať.
3. Vyberte požadovaný typ vzdialeného vymazania údajov. Možnosť vyradenia odstráni len informácie organizácie, zatiaľ čo úplné vymazanie údajov obnoví výrobné nastavenia zariadenia.
4. Výber potvrďte kliknutím na tlačidlo **Áno**. Kým sa vymazanie nedokončí, stav akcie Zariadenie sa zobrazuje ako *Čaká sa na vyradenie*.
    Po dokončení akcie sa mobilné zariadenie už v zozname spravovaných zariadení nebude nachádzať.

**Poznámka:** Údaje spoločnosti nemožno odstrániť zo zariadení pripojených k službe Azure AD. 

Úplné podrobnosti o vplyve akcií Vyradeniie a Vymazanie vrátane toho, čo sa zachová a čo sa odstráni, nájdete v nasledujúcej dokumentácii:

- [Odstránenie zariadení pomocou vymazania, vyradenia alebo manuálneho zrušenia registrácie](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Vymazanie len podnikových údajov z aplikácií spravovaných službou Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Vymazanie všetkých údajov zo zariadenia so systémom macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).