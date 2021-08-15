---
title: Chyby synchronizácie automatickej registrácie zariadenia Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013763"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby synchronizácie automatickej registrácie zariadenia Apple

Zistili sme, že máte jeden alebo viacero tokenov ADE/DEP, ktoré sú v chybovom stave. Kým sa problém nevyrieši pre každý ovplyvnený token, funkčnosť ADE nebude fungovať podľa očakávaní.

Táto chyba sa môže prejaviť niekoľkými spôsobmi:

1. Zariadenia sa nemusia synchronizovať zo služby ABM/ASM do služby Intune
2. Priradenia profilu registrácie môžu zlyhať
3. Zariadenia možno úspešne dokončili registráciu ADE

Skontrolujte chybu synchronizácie nahlásená v konzole Intune v časti Zariadenia > Zaregistrovať zariadenia > zaregistrovaných **> tokenoch programu Enrollment.**

Jednou z najčastejších príčin chyby synchronizácie je uplynutie platnosti aktuálneho tokenu. V mnohých prípadoch problém vyrieši obnovenie ovplyvneného tokenu.

Ak platnosť jedného alebo viacerých tokenov uplynula, pozrite si nasledujúcu dokumentáciu, ktorá vám ich podľa potreby pomôže obnoviť:

[Obnovenie tokenu registrácie automatického zariadenia](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Okrem toho si môžete pozrieť aj nasledujúcu dokumentáciu na zobrazenie možných opravných krokov pre iné chyby spôsobujúce zlyhania synchronizácie tokenov:

[Chyby synchronizácie ABM/ASM pre iOS/iPadOS a automatizované tokeny registrácie zariadenia v systéme macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Chyby synchronizácie ABM/ASM pre iOS/iPadOS a automatizované tokeny registrácie zariadenia v systéme macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
