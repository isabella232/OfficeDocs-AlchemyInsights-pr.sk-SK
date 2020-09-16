---
title: Používanie e-mailových profilov so službou Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653303"
---
# <a name="using-email-profiles-with-intune"></a>Používanie e-mailových profilov so službou Intune

Intune sa môže použiť na vytvorenie a nasadenie e-mailových profilov pre natívny (vstavaný) e-mailového klienta na viacerých platformách zariadení.

Informácie o niektorých obmedzeniach, ktoré sú priradené k e-mailovým profilom vrátane spôsobu spracovania prítomnosti existujúcich profilov a odstraňovania e-mailových profilov, nájdete v téme [Pridanie nastavení e-mailu do zariadení pomocou služby Intune](https://docs.microsoft.com/intune/email-settings-configure).

Ďalšie informácie o tom, ako vytvoriť e-mailové profily pre každú platformu zariadenia, nájdete v témach:

[Nastavenie zariadenia s Androidom na konfiguráciu e-mailu, overovania a synchronizácie v službe Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Pridanie nastavení e-mailu pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavenie e-mailového profilu v službe Microsoft Intune pre zariadenia s operačným systémom Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavenie e-mailového profilu pre zariadenia s Windowsom 10 v službe Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Bežný problém so synchronizáciou**

**Platforma KNOX v e-mailovom profile pre Android zabraňuje synchronizácii používateľských kontaktov, kalendára a úloh v synchronizácii s používateľskými zariadeniami.**

E-mailový profil KNOX v systéme Android KNOX poskytuje správcovi možnosť rozhodnúť sa, ktoré typy obsahu sa synchronizujú so zariadením, nastavením jednotlivých povolení.

Ak je nastavenie pre ktorýkoľvek z typov obsahu nastavené na možnosť **nie je nakonfigurované** (predvolené), daný typ obsahu sa nesynchronizuje automaticky. Používateľ môže povoliť manuálne nastavenie typu obsahu priamo v zariadení, ale táto konfigurácia sa prepíše nastavením politiky služby Intune a synchronizácia sa prestane pre daný typ obsahu.

