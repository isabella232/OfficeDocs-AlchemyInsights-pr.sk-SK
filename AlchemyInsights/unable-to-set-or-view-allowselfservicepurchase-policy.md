---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735214"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase

Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase sa zobrazí nasledujúce chybové hlásenie:

*HandleError: Nepodarilo sa načítať politiku produktov s PolicyId ' AllowSelfServicePurchase ', ErrorMessage-základné pripojenie bolo ukončené: na odoslanie sa vyskytla neočakávaná chyba.*

Môže to byť spôsobené staršou verziou zabezpečenia Transport Layer (TLS). Ak chcete pripojiť službu MSCommerce, musíte použiť TLS 1,2 alebo novšiu.  

Vyskúšajte nasledujúce kroky na zapnutie alebo nastavenie protokolu TLS na 1,2, overenie a opakovanie.
 1. V príkazovom riadku prostredia PowerShell (PS C: \) Ak chcete nastaviť protokol TLS na verziu 1,2, zadajte nasledujúci príkaz:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Overte, či sa používajú protokoly TLS s týmto príkazom:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Podľa potreby zopakujte príkazy získať alebo aktualizovať.

