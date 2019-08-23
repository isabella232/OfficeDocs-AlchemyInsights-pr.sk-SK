---
title: Práca s iOS VPP aplikácie pravidla Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558020"
---
# <a name="working-with-ios-vpp-applications"></a>Práca s iOS VPP aplikácie

Čítať [ako zvládať iOS aplikácie zakúpené prostredníctvom programu objem nákupu s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) sa dozvedieť o funkcie, obmedzenia a kroky, aby sa Apple objem nákupu Program a podporu pre to v Microsoft Intune.
  
 **Spoločné otázky:** "IOS VPP aplikácie priradené používateľom, ale Inštalácia zlyhala."
  
- To môže nastať ak jeden token VPP sa používa vo viacerých poskytovateľov riešení na správu mobilných zariadení. VPP tokeny od Apple môže byť použité iba s jedným poskytovateľom. Ak ste použili VPP token s viacerými poskytovateľmi, musí re-upload token Windows Intune.

- Inštalácia tiež môže zlyhať, ak celkový počet zariadení presiahnuť počet licencií. Zobraziť zostavy používania pre vaše licencie, prejdite na **Windows Intune mobilné aplikácie** \> stránke **aplikácie licencie** . Naučiť sa kultivovať licencií používaných, pozri [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
