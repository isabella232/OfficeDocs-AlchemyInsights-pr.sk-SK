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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="c0a26-102">Chyby synchronizácie pre automatické zaregistrované zariadenia Apple</span><span class="sxs-lookup"><span data-stu-id="c0a26-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="c0a26-103">"Zistili sme, že máte jeden alebo viacero tokenov ADE/DEP, ktoré sú v chybovom stave.</span><span class="sxs-lookup"><span data-stu-id="c0a26-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="c0a26-104">Kým sa stav chyby nevyrieši pre každý príslušný token, funkcia ADE nebude fungovať podľa očakávaní.</span><span class="sxs-lookup"><span data-stu-id="c0a26-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="c0a26-105">Táto chyba sa môže prejaviť viacerými spôsobmi, napríklad:</span><span class="sxs-lookup"><span data-stu-id="c0a26-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="c0a26-106">Zariadenia sa nemusia synchronizovať z ABM/ASM do služby Intune</span><span class="sxs-lookup"><span data-stu-id="c0a26-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="c0a26-107">Priradenia profilu registrácie sa môžu nedarí</span><span class="sxs-lookup"><span data-stu-id="c0a26-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="c0a26-108">Zariadenia nemusia úspešne vykonať registráciu ADE.</span><span class="sxs-lookup"><span data-stu-id="c0a26-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="c0a26-109">Skontrolujte, či je chyba synchronizácie hlásená v konzole Intune v časti **zariadenia > zapísať zariadenia > registráciu Apple > programové tokeny registrácie**.</span><span class="sxs-lookup"><span data-stu-id="c0a26-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="c0a26-110">Jednou z najčastejších príčin chyby synchronizácie je uplynutie platnosti aktuálneho tokenu.</span><span class="sxs-lookup"><span data-stu-id="c0a26-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="c0a26-111">V mnohých prípadoch sa problém vyrieši obnovením príslušného tokenu.</span><span class="sxs-lookup"><span data-stu-id="c0a26-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="c0a26-112">Ak uplynula platnosť jedného alebo viacerých tokenov, pozrite si nasledujúcu dokumentáciu, ktorá vám pomôže obnoviť ich podľa potreby:</span><span class="sxs-lookup"><span data-stu-id="c0a26-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="c0a26-113">Obnovenie tokenu automatického registrácie zariadenia</span><span class="sxs-lookup"><span data-stu-id="c0a26-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="c0a26-114">Okrem toho môžete zobraziť nasledujúcu dokumentáciu s cieľom Zobraziť možné nápravy pri iných chybách spôsobujúcich zlyhanie synchronizácie tokenov:</span><span class="sxs-lookup"><span data-stu-id="c0a26-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="c0a26-115">Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS</span><span class="sxs-lookup"><span data-stu-id="c0a26-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="c0a26-116">Chyby synchronizácie v rámci ABM/ASM pre automatizované tokeny registrácie zariadenia so systémom iOS/iPadOS a macOS</span><span class="sxs-lookup"><span data-stu-id="c0a26-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
