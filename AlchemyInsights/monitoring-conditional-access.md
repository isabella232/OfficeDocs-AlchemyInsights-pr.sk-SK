---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902376"
---
# <a name="monitoring-conditional-access"></a>Monitorovanie podmieneného prístupu

Užívatelia cielené s podmieneným prístupom dostane e-mail s upozornením, ak nespĺňajú požiadavky vašej organizácie. Ak chcete vyriešiť, odporúčame jeden alebo viac z nasledujúcich riešení:
  
- Ak zariadenie predpokladá sa zapísal, poradiť užívateľovi ísť k aplikácie portáli spoločnosti a overte, že sa zdá, na portáli spoločnosti. Ak to tak nie je, používateľ by mal zapísať zariadenia.
    
- Na portáli Azure ísť do **Intune \> zariadenia súlad**. Pod **monitorom s** kliknite na **zariadenie súladu**. Zobrazenia zostavy súladu zariadení na overenie, že zariadenie používateľa je označená ako vyhovujúce. 
    
- Na portáli Azure ísť do **Intune \> zariadenia súlad**. Podľa **Spravovať**, kliknite na položku **politiky**. V zozname súladu politík, overiť, že profil je priradený k zariadení vášho používateľa. Ak je priradený žiadny profil, potom Intune nebude schopný potvrdiť zhodu stav zariadenia. 
    
- Upraviť priradenie podmieneného prístupu.
    
1. Na portáli Azure ísť do **Intune \> podmieneného prístupu \> podmienky**
    
2. Zo zoznamu vyberte politiku
    
3. Kliknite na tlačidlo **používateľov a skupín**
    
4. Osloviť určitú politiku na niekoho pridať do zoznamu pre **zahrnutie** . Zabezpečiť, že osoba je vynechaný z politiky, pridajte ich do zoznamu **vylúčenie** . 
    
Prečítajte si viac: [ako Monitor podmieneného prístupu zariadenia](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

