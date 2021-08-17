---
title: Working with iOS VPP Applications Rule Id 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083029"
---
# <a name="working-with-ios-vpp-applications"></a>Práca s aplikáciami VPP systému iOS

Prečítajte si informácie o funkciách, obmedzeniach a krokoch na používanie programu Apple Volume Purchase a podpory pre tento program v programe balíka Microsoft Intune. Prečítajte si článok Spravovanie aplikácií systému iOS zakúpených prostredníctvom multiliclicného programu so systémom [Microsoft Intune Microsoft Intune.](https://docs.microsoft.com/intune/vpp-apps-ios)
  
 **Bežné problémy:** Používateľom bola priradená aplikácia VPP systému iOS, ale inštalácia zlyhala.
  
- Môže sa to stať, ak sa jeden token VPP použije v rámci viacerých poskytovateľov správy mobilných zariadení. Tokeny VPP od spoločnosti Apple sa môžu používať len s jedným poskytovateľom. Ak ste používali token VPP s viacerými poskytovateľmi, token je potrebné znova nahrať do služby Intune.

- Inštalácia môže zlyhať aj vtedy, ak celkový počet inštalácií prekročí počet licencií. Ak chcete zobraziť zostavu o používaní svojich licencií, prejdite na stránku Licencie na **aplikácie intune** \>  Mobile. Informácie o tom, ako získať opätovné využitie licencií, nájdete v [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
