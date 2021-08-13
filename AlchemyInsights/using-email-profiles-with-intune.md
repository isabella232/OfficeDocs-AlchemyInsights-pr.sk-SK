---
title: Používanie e-mailových profilov v intune
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919438"
---
# <a name="using-email-profiles-with-intune"></a>Používanie e-mailových profilov v intune

Intune možno použiť na vytvorenie a nasadenie e-mailových profilov pre natívne (vstavané) e-mailového klienta na viacerých platformách zariadení.

Informácie o niektorých obmedzeniach súvisiacich s e-mailovými profilmi vrátane spôsobu manipulácie s prítomnosťou existujúcich profilov a odstránenia e-mailových profilov nájdete v téme Pridanie nastavení e-mailu do zariadení po použití [služby Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Ďalšie informácie o vytváraní e-mailových profilov pre platformy jednotlivých zariadení nájdete v týchto téme:

[Nastavenia zariadenia s Androidom na konfiguráciu e-mailu, overovania a synchronizácie v Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Pridanie e-mailových nastavení pre zariadenia so systémom iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavenia e-mailového profilu v Microsoft Intune pre zariadenia so Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavenia e-mailového profilu pre zariadenia so Windows 10 v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Bežný problém so synchronizáciou**

**KNOX v e-mailovom profile Androidu zabraňuje používateľom v synchronizácii kontaktov, kalendára a úloh s používateľskými zariadeniami.**

Funkcia KNOX v e-mailovom profile systému Android KNOX poskytuje správcom možnosť rozhodnúť sa, ktoré typy obsahu sa majú so zariadením synchronizovať, nastavením ich zapnutých.

Ak je nastavenie pre niektorý z typov obsahu nastavené na hodnotu Nie je **nakonfigurované** (predvolené), tento typ obsahu sa nesynchronizuje automaticky. Používateľ môže povoliť typ obsahu, ktorý chce, priamo v zariadení, ale toto nastavenie sa prepíše nastavením politiky služby Intune a synchronizácia sa pre tento typ obsahu zastaví.

