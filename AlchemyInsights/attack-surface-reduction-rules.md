---
title: Pravidlá zmenšenia oblasti útokov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676442"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="8bee8-102">Pravidlá zmenšenia oblasti útokov</span><span class="sxs-lookup"><span data-stu-id="8bee8-102">Attack surface reduction rules</span></span>

<span data-ttu-id="8bee8-103">Vylúčenie súborov alebo priečinkov môže vážne znížiť ochranu, ktorú poskytujú pravidlá na zníženie počtu útokov v oblasti povrchov.</span><span class="sxs-lookup"><span data-stu-id="8bee8-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="8bee8-104">Súbory, ktoré by boli zablokované pravidlom, môžu byť spúšťané a nezaehrajú sa žiadne zostavy ani udalosti.</span><span class="sxs-lookup"><span data-stu-id="8bee8-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="8bee8-105">Vylúčenie sa vzťahuje na všetky pravidlá, ktoré umožňujú vylúčenie.</span><span class="sxs-lookup"><span data-stu-id="8bee8-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="8bee8-106">Vylúčenia ASR používajú rovnakú syntax ako vo Microsoft Defender Antivirus vylúčenia.</span><span class="sxs-lookup"><span data-stu-id="8bee8-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="8bee8-107">Podrobnosti nájdete v téme [Konfigurácia a overenie vylúčení pre Microsoft Defender Antivirus kontroly.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="8bee8-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="8bee8-108">Ak sa chcete vyhnúť problémom, [pozrite si bežné chyby, ktorým sa vyhnete pri definovaní vylúčení](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="8bee8-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="8bee8-109">Nie všetky pravidlá ASR podporujú vylúčenia.</span><span class="sxs-lookup"><span data-stu-id="8bee8-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="8bee8-110">Ak chcete overiť, či vaše pravidlo podporuje vylúčenia, pozrite si tabuľku Pravidlá pre zníženie počtu miest útokov na [povrchu.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="8bee8-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="8bee8-111">Pravidlá zmenšenia oblasti útokov</span><span class="sxs-lookup"><span data-stu-id="8bee8-111">Attack surface reduction rules</span></span>

<span data-ttu-id="8bee8-112">Útok na ploche vašej organizácie zahŕňa všetky miesta, kde útočník mohol ohroziť organizačné zariadenia alebo siete.</span><span class="sxs-lookup"><span data-stu-id="8bee8-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="8bee8-113">Zníženie počtu miest útokov znamená ochranu zariadení a siete v organizácii, ktorá vnechá útoky menším spôsobom.</span><span class="sxs-lookup"><span data-stu-id="8bee8-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="8bee8-114">Pomôcť môže konfigurácia pravidiel na zníženie počtu útokov v programe Microsoft Defender pre koncový bod.</span><span class="sxs-lookup"><span data-stu-id="8bee8-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="8bee8-115">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="8bee8-115">For more information, see:</span></span>

- [<span data-ttu-id="8bee8-116">Priradenie identifikátora GUID pravidla ASR k názvu</span><span class="sxs-lookup"><span data-stu-id="8bee8-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="8bee8-117">Požiadavky pravidiel ASR:</span><span class="sxs-lookup"><span data-stu-id="8bee8-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="8bee8-118">Windows 10 Pro, verzia 1709 alebo novšia</span><span class="sxs-lookup"><span data-stu-id="8bee8-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="8bee8-119">Windows 10 Enterprise, verzia 1709 alebo novšia</span><span class="sxs-lookup"><span data-stu-id="8bee8-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="8bee8-120">Windows Server, verzia 1803 (polročné kanály) alebo novšia</span><span class="sxs-lookup"><span data-stu-id="8bee8-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="8bee8-121">Identifikácia správneho vylúčenia, ktoré je potrebné použiť</span><span class="sxs-lookup"><span data-stu-id="8bee8-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="8bee8-122">V denníku eventID 1121 alebo 1122 vyhľadajte položku eventID 1122 Windows-Windows Defender/Operational.</span><span class="sxs-lookup"><span data-stu-id="8bee8-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="8bee8-123">Vyhodnoťte scenár blokovania a kontext a potvrďte, že tento scenár je potrebné odblokovať.</span><span class="sxs-lookup"><span data-stu-id="8bee8-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="8bee8-124">Prečítajte si hodnotu Cesta v podrobnostiach udalosti, čo je hodnota, ktorá definuje vylúčenie.</span><span class="sxs-lookup"><span data-stu-id="8bee8-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="8bee8-125">Vylúčenie vykonajte čo najprísnejšie.</span><span class="sxs-lookup"><span data-stu-id="8bee8-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="8bee8-126">V prípade potreby použite zástupný znak (napríklad nahraďte premennú Používateľa).</span><span class="sxs-lookup"><span data-stu-id="8bee8-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="8bee8-127">Vylúčenie použite podľa potrieb nasadenia.</span><span class="sxs-lookup"><span data-stu-id="8bee8-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="8bee8-128">Podrobné informácie nájdete v téme [Prispôsobenie pravidiel na zníženie počtu útokov v povrchovom zariadení.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="8bee8-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="8bee8-129">Vylúčenie nie je ocenené</span><span class="sxs-lookup"><span data-stu-id="8bee8-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="8bee8-130">Určite, či pravidlo podporuje vylúčenia.</span><span class="sxs-lookup"><span data-stu-id="8bee8-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="8bee8-131">Podrobnosti nájdete v téme Pravidlá [na zníženie počtu povrchov útokov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="8bee8-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="8bee8-132">Skontrolujte použité vylúčenia a v údajoch udalosti overte preklepy alebo nesprávne použité zástupné znaky.</span><span class="sxs-lookup"><span data-stu-id="8bee8-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="8bee8-133">Ďalšie informácie nájdete v téme [Podporované typy vylúčenia.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="8bee8-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="8bee8-134">ak je vplyv pravidla príliš vysoký, zvážte presunutie pravidla (späť) do režimu auditu a vykonanie ďalšieho overenia.</span><span class="sxs-lookup"><span data-stu-id="8bee8-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="8bee8-135">Podrobnosti nájdete v téme [Testovanie funkcií Microsoft Defendera pre koncové body v režime auditu.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="8bee8-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="8bee8-136">Zhromaždite údaje podpory na otvorenie prípadu podpory pomocou tohto príkazu:</span><span class="sxs-lookup"><span data-stu-id="8bee8-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="8bee8-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="8bee8-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="8bee8-138">Ďalšie informácie nájdete v téme [Problémy s onboarding zariadeniami s aplikáciou Microsoft Defender pre koncové body.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="8bee8-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
