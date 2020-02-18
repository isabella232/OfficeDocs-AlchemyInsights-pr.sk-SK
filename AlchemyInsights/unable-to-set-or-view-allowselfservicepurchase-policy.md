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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091762"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase

Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase, zobrazí nasledujúce chybové hlásenie:

*HandleError: Nepodarilo sa načítať politiku produktu s PolicyId "AllowSelfServicePurchase", ErrorMessage-základné pripojenie bolo zatvorené: Vyskytla sa neočakávaná chyba pri odosielaní.*

Môže to byť spôsobené staršou verziou zabezpečenia transportnej vrstvy (TLS). Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1,2 alebo vyšší.  

Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na 1,2, overenie a opakovanie.
 1. V príkazovom riadku prostredia PowerShell (PS C:\) zadajte nasledovný príkaz na nastavenie protokolu TLS na verziu 1,2:

    \[NET. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12

2. Overte, či protokol (y) TLS používa, s nasledujúcim príkazom:

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Podľa potreby zopakujte príkazy získať alebo aktualizovať.

