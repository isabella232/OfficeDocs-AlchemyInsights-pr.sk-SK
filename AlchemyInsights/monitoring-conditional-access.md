---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708689"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorovanie podmieneného prístupu pre Exchange

Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie. Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:

- Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli. Ak to tak nie je, používateľ by mal zariadenie zaregistrovať.
- Na portáli Azure prejdite do služby Intune > súladu zariadenia. V časti monitor kliknite na položku súlad zariadenia. Ak chcete overiť, či je zariadenie používateľa označené ako vyhovujúce, pozrite si zostavu súladu zariadenia.
- Na portáli Azure prejdite do služby Intune > súladu zariadenia. V časti Spravovať kliknite na položku politiky. V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa. Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia.
- Upravte priradenie podmieneného prístupu používateľa.

1. Na portáli Azure prejdite na   >  **politiky podmieneného prístupu** služby Intune  >  .
2. Zo zoznamu vyberte politiku.
3. Kliknite na položku Používatelia a skupiny.
4. Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do zoznamu zahrnúť. Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do zoznamu výnimiek.

Užitočné prepojenia:

[Prehľad súladu zariadenia](https://docs.microsoft.com/intune/device-compliance-get-started)

[Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politika riešenia problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Sledovanie dodržiavania súladu zariadenia Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Poznámka: tieto kroky sú užitočné len pri riešení problémov s podmieneným prístupom funkcie Azure Active Directory. Je tiež možné do karantény zablokovať zariadenie, ktoré blokuje prístup k e-mailu pomocou politiky Exchange. Ďalšie informácie o spravovaní zariadení s Exchangeom nájdete v téme [tu] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
