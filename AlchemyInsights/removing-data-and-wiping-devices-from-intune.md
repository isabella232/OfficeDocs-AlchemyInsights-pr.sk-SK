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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922267"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odstránenie údajov a vymazanie zariadení z Intune

Vzdialené akcie Vyradenie zariadenia a Vymazanie zariadenia možno použiť na odstránenie podnikových údajov spravovaných službou Intune alebo na resetovanie výrobných nastavení a obnovenie predvolených nastavení zariadenia.

1. Prihláste sa do aplikácie Správa zariadení pre Microsoft 365 a prejdite na položku **Zariadenia** > **Všetky zariadenia**.
2. Vyberte zariadenie, v ktorom chcete údaje vymazať.
3. Vyberte požadovaný typ vzdialeného vymazania údajov. Možnosť vyradenia odstráni len informácie organizácie, zatiaľ čo úplné vymazanie údajov obnoví výrobné nastavenia zariadenia.
4. Výber potvrďte kliknutím na tlačidlo **Áno**. Kým sa vymazanie nedokončí, stav akcie Zariadenie sa zobrazuje ako *Čaká sa na vyradenie*.
    Po dokončení akcie sa mobilné zariadenie už v zozname spravovaných zariadení nebude nachádzať.

> [!NOTE]
> Údaje spoločnosti nie je možné odstrániť zo zariadení PRIPOJENÝCH do služby Azure AD. 

Úplné podrobnosti o vplyve akcií Vyradeniie a Vymazanie vrátane toho, čo sa zachová a čo sa odstráni, nájdete v nasledujúcej dokumentácii:

- [Odstránenie zariadení pomocou vymazania, vyradenia alebo manuálneho zrušenia registrácie](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Vymazanie len podnikových údajov z aplikácií spravovaných službou Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Vymazanie všetkých údajov zo zariadenia so systémom macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).