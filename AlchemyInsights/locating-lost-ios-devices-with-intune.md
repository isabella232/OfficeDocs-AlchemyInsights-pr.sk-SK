---
title: Vyhľadanie stratených zariadení so systémom iOS pomocou intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440428"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Vyhľadanie stratených zariadení so systémom iOS pomocou intune

Povolenie režimu strateného v zariadení so systémom iOS umožňuje správcovi zobraziť správu a telefónne číslo kontaktu na obrazovke uzamknutia.

Po povolení režimu strateného môže správca použiť akciu Vyhľadať zariadenie na identifikáciu fyzického umiestnenia zariadenia.

Akcia Vyhľadať zariadenie v programe Intune funguje so zariadeniami so systémom iOS a zobrazí umiestnenie konkrétneho zariadenia na mape.

Použitie tejto akcie vyžaduje, aby sa zariadenie so systémom iOS nachádzali v:

- Režim pod dohľadom
- Režim straty

Ďalšie informácie nájdete v téme [Povolenie strateného režimu v zariadeniach so systémom iOS/iPadOS so zariadeniami Intune](https://docs.microsoft.com/intune/device-lost-mode) a Vyhľadanie stratených alebo odcudzených [zariadení so systémom iOS/iPadOS so systémom Intune](https://docs.microsoft.com/intune/device-locate).

**Najčastejšie otázky**

Otázka: Vydal som vzdialenú akciu na odstránenie údajov spoločnosti zo zariadenia a teraz je uviaznutá v stave čakajúceho.

A: Ak chcete úspešne dokončiť vzdialenú akciu, cieľové zariadenie musí byť online a zdravé. V nasledujúcich situáciách, vzdialená akcia zostane v stave čakania po dobu 30 dní, alebo kým zariadenie potvrdí príkaz:

- Keï prístroj nemá konektivitu,
- Keď zariadenie stratí stav správy pomocou intune

Ak si myslíte, že zariadenie už nie je v e-v zariadení v e-tom a nebude môcť odstrániť údaje spoločnosti, vyberte položku Odstrániť. Odstránením sa odstráni záznam zariadenia tak, aby sa už nestraší v zozname zariadení Intune. Ak sa zariadenie znova aktivuje, jeho používateľ ho bude musieť znova zaregistrovať.

Otázka: Prečo nie sú niektoré vzdialené akcie dostupné na používanie?

A: Nie všetky platformy podporujú všetky akcie vzdialeného zariadenia. Nasledujúce vzdialené akcie sú špecifické pre platformu, takže sú k dispozícii len pre zaznamenané platformy.

- Obísť zámok aktivácie (len pre iOS)
- Nový začiatok (len v systéme Windows)
- Režim straty (len pre iOS)
- Vyhľadanie zariadenia (len pre iOS)
- Reštartovať (len v systéme Windows)

Ďalšie podrobnosti o jednotlivých akciách nájdete v téme [Akcie dostupného zariadenia](https://docs.microsoft.com/intune/device-management#available-device-actions).