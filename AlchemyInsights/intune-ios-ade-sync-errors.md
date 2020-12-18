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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="98588-102">Chyby synchronizácie pre automatické zaregistrované zariadenia Apple</span><span class="sxs-lookup"><span data-stu-id="98588-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="98588-103">"Zistili sme, že máte jeden alebo viacero tokenov ADE/DEP, ktoré sú v chybovom stave.</span><span class="sxs-lookup"><span data-stu-id="98588-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="98588-104">Kým sa stav chyby nevyrieši pre každý príslušný token, funkcia ADE nebude fungovať rovnako.</span><span class="sxs-lookup"><span data-stu-id="98588-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="98588-105">Táto chyba sa môže prejaviť viacerými spôsobmi, napríklad:</span><span class="sxs-lookup"><span data-stu-id="98588-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="98588-106">Zariadenia sa nemusia synchronizovať z ABM/ASM do služby Intune</span><span class="sxs-lookup"><span data-stu-id="98588-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="98588-107">Priradenia profilu registrácie sa môžu nedarí</span><span class="sxs-lookup"><span data-stu-id="98588-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="98588-108">Zariadenia nemusia úspešne vykonať registráciu ADE.</span><span class="sxs-lookup"><span data-stu-id="98588-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="98588-109">Skontrolujte, či je chyba synchronizácie hlásená v konzole Intune v časti **zariadenia > zapísať zariadenia > registráciu Apple > programové tokeny registrácie** a prečítajte si nasledujúcu dokumentáciu, aby sa zobrazili prípadné prípadné nápravy:</span><span class="sxs-lookup"><span data-stu-id="98588-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="98588-110">Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS</span><span class="sxs-lookup"><span data-stu-id="98588-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
