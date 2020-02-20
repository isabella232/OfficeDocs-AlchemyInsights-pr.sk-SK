---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158576"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase

Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase, zobrazí nasledujúce chybové hlásenie:

*HandleError: Nepodarilo sa načítať politiku produktu s PolicyId "AllowSelfServicePurchase", ErrorMessage-základné pripojenie bolo zatvorené: Vyskytla sa neočakávaná chyba pri odosielaní.*

Môže to byť spôsobené staršou verziou zabezpečenia transportnej vrstvy (TLS). Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1,2 alebo vyšší.  

Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na 1,2, overenie a opakovanie.
 1. V príkazovom riadku prostredia PowerShell (PS C:\) zadajte nasledovný príkaz na nastavenie protokolu TLS na verziu 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Overte, či protokol (y) TLS používa, s nasledujúcim príkazom:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Podľa potreby zopakujte príkazy získať alebo aktualizovať.

