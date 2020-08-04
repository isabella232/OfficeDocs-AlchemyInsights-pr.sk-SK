---
title: Používanie e-mailových profilov s intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555762"
---
# <a name="using-email-profiles-with-intune"></a>Používanie e-mailových profilov s intune

Intune možno vytvoriť a nasadiť e-mailové profily pre natívne (vstavaný) e-mailový klient na viacerých platformách zariadení.

Informácie o niektorých obmedzeniach súvisiacich s e-mailovými profilmi vrátane spôsobu spracovania prítomnosti existujúcich profilov a spôsobu odstránenie e-mailových profilov nájdete v téme [Pridanie nastavení e-mailu do zariadení pomocou aplikácie Intune](https://docs.microsoft.com/intune/email-settings-configure).

Ďalšie informácie o vytváraní e-mailových profilov pre každú platformu zariadení nájdete v téme:

[Nastavenia zariadenia s Androidom na konfiguráciu e-mailov, overovania a synchronizácie v programe Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Pridanie nastavení e-mailu pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavenia e-mailového profilu v službe Microsoft Intune pre zariadenia so systémom Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavenie e-mailového profilu pre zariadenia so systémom Windows 10 v microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Bežný problém so synchronizáciou**

**Knox v e-mailovom profile Androidu zabraňuje synchronizácii kontaktov, kalendára a úloh používateľa s používateľskými zariadeniami.**

E-mailový profil KNOX v systéme Android KNOX ponúka správcovi možnosť rozhodnúť sa, ktoré typy obsahu sa synchronizujú so zariadením, nastavením každého na povolené.

Ak je nastavenie pre niektorý z typov obsahu nastavené na možnosť **Nie je nakonfigurované** (predvolené), tento typ obsahu sa nesynchronizuje automaticky. Používateľ môže zapnúť typ obsahu, ktorý chcete priamo v zariadení manuálne, ale táto konfigurácia sa prepíše nastavením politiky Intune a synchronizácia sa zastaví pre tento typ obsahu.

