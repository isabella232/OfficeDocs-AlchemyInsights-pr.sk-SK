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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702918"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorovanie podmieneného prístupu pre Exchange

Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie. Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:
  
- Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli. Ak to tak nie je, používateľ by mal zariadenie zaregistrovať.
    
- Na portáli Azure prejdite na ** \> súlad zariadenia**so službou Intune. V časti **Monitor** kliknite na položku **súlad zariadenia**. Ak chcete overiť, či je zariadenie používateľa označené ako vyhovujúce, pozrite si zostavu súladu zariadenia. 
    
- Na portáli Azure prejdite na ** \> súlad zariadenia**so službou Intune. V časti **Spravovať**kliknite na položku **politiky**. V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa. Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia. 
    
- Upravte priradenie podmieneného prístupu používateľa.
    
1. Na portáli Azure prejdite na ** \> \> politiky podmieneného prístupu služby Intune**
    
2. Výber politiky v zozname
    
3. Kliknite na položku **Používatelia a skupiny**
    
4. Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do zoznamu **zahrnúť** . Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do zoznamu **výnimiek** . 
    
Ďalšie informácie: [ako sledovať zariadenia s podmieneným prístupom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

