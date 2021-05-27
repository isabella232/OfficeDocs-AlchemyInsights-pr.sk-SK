---
title: Indikátory nefungujú v prehliadači Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676466"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="8eda1-102">Indikátory nefungujú v prehliadači Edge</span><span class="sxs-lookup"><span data-stu-id="8eda1-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="8eda1-103">Po vytvorení indikátora sa aplikácia neminie podľa okraja (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="8eda1-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="8eda1-104">Ďalšie informácie nájdete v téme [Vytváranie indikátorov IP adries a URL adries alebo domén.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="8eda1-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="8eda1-105">Krok 1: Uistite sa, že:</span><span class="sxs-lookup"><span data-stu-id="8eda1-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="8eda1-106">Overte správnosť indikátora (žiadne preklepy v IP/URL, správna akcia, správne skupiny pre RBAC).</span><span class="sxs-lookup"><span data-stu-id="8eda1-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="8eda1-107">Po vytvorení indikátora počkajte minimálne 2 hodiny, aby sa zohľadňovať prípadné časové oneskorenie.</span><span class="sxs-lookup"><span data-stu-id="8eda1-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="8eda1-108">Skontrolujte, či sú systém (systém) v aplikácii Microsoft Defender pre koncový bod k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="8eda1-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="8eda1-109">Overte, či môžu systém (či) komunikovať s cloudom.</span><span class="sxs-lookup"><span data-stu-id="8eda1-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="8eda1-110">Na testovacej lokalite overte, či je obrazovka SmartScreen povolená a [dostupná.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="8eda1-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="8eda1-111">Krok 2: Riešenie potenciálneho problému</span><span class="sxs-lookup"><span data-stu-id="8eda1-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="8eda1-112">Uistite sa, že klient spĺňa požiadavky.</span><span class="sxs-lookup"><span data-stu-id="8eda1-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="8eda1-113">Podrobnosti nájdete v téme [Vytváranie indikátorov IP adries a URL adries alebo domén.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="8eda1-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="8eda1-114">Uistite sa, že používate najnovšiu verziu prehliadača Edge.</span><span class="sxs-lookup"><span data-stu-id="8eda1-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="8eda1-115">Ak chcete zistiť najnovšiu verziu, pozrite [si časť Zistite, ktorú verziu balíka Microsoft Edge používate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="8eda1-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="8eda1-116">Reštartujte prehliadač Edge.</span><span class="sxs-lookup"><span data-stu-id="8eda1-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="8eda1-117">Prejdite na lokalitu, pre ktorú máte nastavenie indikátora.</span><span class="sxs-lookup"><span data-stu-id="8eda1-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="8eda1-118">Ak sa lokalita nezobrazuje podľa očakávania, pokračujte krokom 3.</span><span class="sxs-lookup"><span data-stu-id="8eda1-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="8eda1-119">Krok 3: Zhromažďovanie údajov</span><span class="sxs-lookup"><span data-stu-id="8eda1-119">Step 3: Collect data</span></span>

- <span data-ttu-id="8eda1-120">Zhromažďovanie **diagnostických údajov MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="8eda1-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="8eda1-121">Pokyny nájdete v téme [Problémy s onboardingami v aplikácii Microsoft Defender pre koncový bod.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="8eda1-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="8eda1-122">Ak ste si dobre nainštalovali a zhromažďovali sledovanie Fiddler, pozrite si [časť Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="8eda1-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="8eda1-123">Ak uprednostňujete pokyny od podpory spoločnosti Microsoft, výberom ikony podpory nižšie otvorte prípad podpory.</span><span class="sxs-lookup"><span data-stu-id="8eda1-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
