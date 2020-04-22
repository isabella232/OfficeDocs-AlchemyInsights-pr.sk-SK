---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713733"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorovanie podmieneného prístupu pre Exchange

Používatelia zacielené na podmienený prístup dostanú e-mailové upozornenie, ak nespĺňajú požiadavky vašej organizácie na prístup. Ak chcete vyriešiť, odporúčame jedno alebo viaceré z nasledujúcich riešení:
  
- Ak sa predpokladá, že zariadenie je zapísané, radí používateľovi prejsť na firemný portál aplikácie a overiť, že sa zobrazí na portáli spoločnosti. Ak sa tak nestane, používateľ by mal zariadenie zapísať.
    
- V Azure portál prejdite na **zariadenie Intune \> súlad zariadenia**. V časti **Monitor** kliknite na položku **zhoda zariadení**. Zobrazte zostavu súladu so zariadením a overte, či je zariadenie používateľa označené ako vyhovujúce. 
    
- V Azure portál prejdite na **zariadenie Intune \> súlad zariadenia**. V časti **Spravovať**kliknite na položku **politiky**. V zozname politík súladu overte, či je profil priradený zariadeniu používateľa. Ak nie je priradený žiadny profil, Intune nebude môcť potvrdiť stav súladu zariadenia. 
    
- Upravte priradenie podmieneného prístupu používateľa.
    
1. V Azure portál prejsť na **Intune \> podmieneného prístupu \> politiky**
    
2. Vybrať politiku zo zoznamu
    
3. Kliknite na položku **Používatelia a skupiny**
    
4. Ak chcete zacieliť určitú politiku na niekoho, pridajte ich do zoznamu **zahrnúť** . Ak chcete zabezpečiť, aby bola osoba vynechaná z politiky, pridajte ich do zoznamu **výnimiek** . 
    
Čítajte viac: [ako sledovať zariadenia podmieneného prístupu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

