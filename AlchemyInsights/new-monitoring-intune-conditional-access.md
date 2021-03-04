---
title: Monitorovanie podmieneného prístupu služby Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428306"
---
# <a name="monitor-intune-conditional-access"></a>Monitorovanie podmieneného prístupu služby Intune

Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie. Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:

1. Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli. Ak to tak nie je, používateľ musí zaregistrovať zariadenie.
1. Na portáli Azure prejdite na   >  **súlad zariadenia** so službou Intune. 
1. Ak chcete zobraziť zostavu súladu zariadenia a overiť, či je zariadenie používateľa označené ako vyhovujúce, v časti **Monitor** kliknite na položku **zhoda zariadení**.
1. Na portáli Azure prejdite na   >  **súlad zariadenia** so službou Intune. V časti **Spravovať** kliknite na položku **politiky**. V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa. Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia.
1. Upravte priradenie podmieneného prístupu používateľa.
1. Na portáli Azure prejdite do   >  časti politiky **podmieneného prístupu** služby Intune  >  , vyberte politiku v zozname a kliknite na položku **Používatelia a skupiny**.
1. Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do **zoznamu zahrnúť**. Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do **zoznamu výnimiek**.

**Užitočné prepojenia:**

- [Prehľad súladu zariadenia](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Politika riešenia problémov](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Sledovanie dodržiavania súladu zariadenia Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Tieto kroky sú užitočné len pri riešení problémov s podmieneným prístupom funkcie Azure Active Directory. Je tiež možné do karantény zablokovať zariadenie, ktoré blokuje prístup k e-mailu pomocou politiky Exchange. Ďalšie informácie o správe zariadenia Exchange nájdete [**tu**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
