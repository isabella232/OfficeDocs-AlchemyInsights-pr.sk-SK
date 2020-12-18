---
title: Chyby synchronizácie pre automatické zaregistrované zariadenia Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714976"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby synchronizácie pre automatické zaregistrované zariadenia Apple

"Zistili sme, že máte jeden alebo viacero tokenov ADE/DEP, ktoré sú v chybovom stave. Kým sa stav chyby nevyrieši pre každý príslušný token, funkcia ADE nebude fungovať rovnako.

Táto chyba sa môže prejaviť viacerými spôsobmi, napríklad:

1. Zariadenia sa nemusia synchronizovať z ABM/ASM do služby Intune
2. Priradenia profilu registrácie sa môžu nedarí
3. Zariadenia nemusia úspešne vykonať registráciu ADE.

Skontrolujte, či je chyba synchronizácie hlásená v konzole Intune v časti **zariadenia > zapísať zariadenia > registráciu Apple > programové tokeny registrácie** a prečítajte si nasledujúcu dokumentáciu, aby sa zobrazili prípadné prípadné nápravy:

[Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
