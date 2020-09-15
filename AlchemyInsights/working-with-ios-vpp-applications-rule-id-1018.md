---
title: Práca so systémom iOS aplikácie VPP Applications ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688961"
---
# <a name="working-with-ios-vpp-applications"></a>Práca s aplikáciami VPP v systéme iOS

Prečítajte si, [ako spravovať aplikácie systému iOS zakúpené prostredníctvom programu na hromadné](https://docs.microsoft.com/intune/vpp-apps-ios) zakúpenie v službe Microsoft Intune, kde získate informácie o funkciách, obmedzeniach a krokoch, ktoré vám pomôžu využiť program na nákup zväzkov Apple a podporu pre IT v službe Microsoft Intune.
  
 **Bežné problémy:** "Priradenú aplikáciu VPP pre systém iOS pre používateľov, ale Inštalácia zlyhala."
  
- Môže sa to stať, ak sa v rámci viacerých poskytovateľov správy mobilných zariadení používa jeden token VPP. Tokeny VPP od spoločnosti Apple sa môžu používať len s jedným poskytovateľom. Ak ste použili token VPP s viacerými poskytovateľmi, token sa musí znova nahrať do služby Intune.

- Inštalácia môže zlyhať aj v prípade, ak celkový počet inštalácií prekročí počet licencií. Ak chcete zobraziť zostavu používania pre svoje licencie, prejdite na stránku licencie aplikácií pre **mobilné aplikácie Intune** \> **App licenses** . Ak sa chcete dozvedieť, ako sa pri používaní licencií uplatniť, prečítajte si [Tento článok.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
