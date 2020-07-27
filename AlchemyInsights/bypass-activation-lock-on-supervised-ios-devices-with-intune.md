---
title: Bypass activation lock on dohliadal iOS zariadenia s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424213"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bypass activation lock on dohliadal iOS zariadenia s Intune

Možnosť obísť zámok aktivácie v zariadeniach so systémom iOS uľahčuje obnovenie zo scenára, v ktorom používateľ povolí zámok aktivácie v podnikovom zariadení a potom opustí spoločnosť.

Predpoklady na obchádzanie zámku aktivácie zahŕňajú:

- Zariadenie je, že je "pod dohľadom."
- Zámok aktivácie je úspešne povolený pomocou politiky obmedzenia zariadenia systému iOS v intune.

Okrem toho, pri obchádzaní zámku aktivácie by ste mali:

- Fyzicky majú zariadenie, ktoré je vymazané.
- Skopírujte kód pred vydaním vymazanie.

**Upozornenie:** Utrite kód nie je malé a veľké písmená, takže "-" znaky nie sú povinné.

Podrobnosti nájdete v téme [Obídenie zámku aktivácie v zariadeniach so systémom iOS pod dohľadom s intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Najčastejšie otázky**

Otázka: **Vydal som vzdialenú akciu na odstránenie údajov spoločnosti zo zariadenia a teraz je uviaznutá v stave čakajúceho.**

A: Ak chcete úspešne dokončiť vzdialenú akciu, cieľové zariadenie musí byť online a zdravé. V nasledujúcich situáciách, vzdialená akcia zostane v stave čakania po dobu 30 dní, alebo kým zariadenie potvrdí príkaz, keď zariadenie:

- Nemá pripojenie.
- Stratí stav správy s Intune.

Ak si myslíte, že zariadenie už nie je v e-v zariadení v e-tom a neodstráni údaje spoločnosti, vyberte položku Odstrániť. Odstránením sa odstráni záznam zariadenia tak, aby sa už nestraší v zozname zariadení Intune. Aby sa zariadenie znova opäť stalo aktívnym, jeho používateľ musí zariadenie znova zaregistrovať.

Otázka: **Prečo nie sú niektoré vzdialené akcie dostupné na používanie?**

A: Nie všetky platformy podporujú všetky akcie vzdialeného zariadenia. Nasledujúce vzdialené akcie sú špecifické pre platformu.

- Obísť zámok aktivácie (len pre iOS)
- Nový začiatok (len v systéme Windows)
- Režim straty (len pre iOS)
- Vyhľadanie zariadenia (len pre iOS)
- Reštartovať (len v systéme Windows)

Ďalšie podrobnosti o jednotlivých akciách nájdete v téme [Akcie dostupného zariadenia](https://docs.microsoft.com/intune/device-management#available-device-actions).