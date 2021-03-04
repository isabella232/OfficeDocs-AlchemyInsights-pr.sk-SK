---
title: Chyby synchronizácie pre automatické zaregistrované zariadenia Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448937"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby synchronizácie pre automatické zaregistrované zariadenia Apple

"Zistili sme, že máte jeden alebo viacero tokenov ADE/DEP, ktoré sú v chybovom stave. Kým sa stav chyby nevyrieši pre každý príslušný token, funkcia ADE nebude fungovať podľa očakávaní.

Táto chyba sa môže prejaviť viacerými spôsobmi, napríklad:

1. Zariadenia sa nemusia synchronizovať z ABM/ASM do služby Intune
2. Priradenia profilu registrácie sa môžu nedarí
3. Zariadenia nemusia úspešne vykonať registráciu ADE.

Skontrolujte, či je chyba synchronizácie hlásená v konzole Intune v časti **zariadenia > zapísať zariadenia > registráciu Apple > programové tokeny registrácie**.

Jednou z najčastejších príčin chyby synchronizácie je uplynutie platnosti aktuálneho tokenu. V mnohých prípadoch sa problém vyrieši obnovením príslušného tokenu.

Ak uplynula platnosť jedného alebo viacerých tokenov, pozrite si nasledujúcu dokumentáciu, ktorá vám pomôže obnoviť ich podľa potreby:

[Obnovenie tokenu automatického registrácie zariadenia](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Okrem toho môžete zobraziť nasledujúcu dokumentáciu s cieľom Zobraziť možné nápravy pri iných chybách spôsobujúcich zlyhanie synchronizácie tokenov:

[Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
