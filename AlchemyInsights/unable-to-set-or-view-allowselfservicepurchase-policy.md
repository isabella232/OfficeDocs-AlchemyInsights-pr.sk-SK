---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020207"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase

Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase sa zobrazí toto chybové hlásenie:

*HandleError: Nepodarilo sa načítať politiku produktu s nastavením PolicyId 'AllowSelfServicePurchase', ErrorMessage – základné pripojenie sa uzavrelo: Pri odosielaní sa vyskytla neočakávaná chyba.*

Môže to byť spôsobené staršou verziou protokolu TLS (Transport Layer Security). Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1.2 alebo vyššiu.  

Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na možnosť 1.2, overenie a zopakovanie pokusu.
 1. Do príkazového riadka prostredia PowerShell (PS C: zadajte nasledujúci príkaz na nastavenie protokolu \) TLS na verziu 1.2):

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Pomocou nasledujúceho príkazu overte protokol TLS, ktorý sa používa:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Podľa potreby znova skúste príkazy Získať alebo Aktualizovať.

