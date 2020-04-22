---
title: Práca s iOS VPP aplikácie ID pravidla 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719972"
---
# <a name="working-with-ios-vpp-applications"></a>Práca s aplikáciami systému iOS VPP

Prečítajte si, [ako spravovať aplikácie pre iOS zakúpené prostredníctvom programu na nákup zväzku s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) a dozvedieť sa o funkciách, obmedzeniach a krokoch, aby ste mohli využiť program na nákup zväzku Apple a podporu pre ňu v Microsoft Intune.
  
 **Bežné problémy:** "Priradil som aplikáciu iOS VPP k mojim používateľom, ale Inštalácia zlyhala."
  
- Môže sa to stať, ak sa v rámci viacerých poskytovateľov správy mobilných zariadení používa jediný token VPP. Žetóny VPP od spoločnosti Apple sa môžu používať iba s jedným poskytovateľom. Ak ste použili token VPP s viacerými poskytovateľmi, musíte znova odovzdať token Intune.

- Inštalácia môže zlyhať aj v prípade, že celkový počet inštalácií prekročí počet licencií. Ak chcete zobraziť zostavu používania pre svoje licencie, prejdite na stránku **licencie aplikácie** **Intune Mobile Apps** \> . Ďalšie informácie o možnostiach opätovného použitia licencií nájdete v [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
