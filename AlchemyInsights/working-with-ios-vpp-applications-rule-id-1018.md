---
title: Práca s iOS VPP aplikácie pravidla Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488933"
---
# <a name="working-with-ios-vpp-applications"></a>Práca s iOS VPP aplikácie

Čítať [ako zvládať iOS aplikácie zakúpené prostredníctvom programu objem nákupu s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) sa dozvedieť o funkcie, obmedzenia a kroky, aby sa Apple objem nákupu Program a podporu pre to v Microsoft Intune. 
  
 **Spoločné otázky:** "IOS VPP aplikácie priradené používateľom, ale Inštalácia zlyhala." 
  
- To môže nastať ak jeden token VPP sa používa vo viacerých poskytovateľov riešení na správu mobilných zariadení. VPP tokeny od Apple môže byť použité iba s jedným poskytovateľom. Ak ste použili VPP token s viacerými poskytovateľmi, musí re-upload token Windows Intune.
    
- Inštalácia tiež môže zlyhať, ak celkový počet zariadení presiahnuť počet licencií. Zobraziť zostavy používania pre vaše licencie, prejdite na **Windows Intune mobilné aplikácie** \> stránke **aplikácie licencie** . Naučiť sa kultivovať licencií používaných, pozri [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

