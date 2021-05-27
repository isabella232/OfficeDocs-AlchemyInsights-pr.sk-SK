---
title: Riešenie chýb blokovania ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676282"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="01290-102">Riešenie chýb blokovania ediscovery</span><span class="sxs-lookup"><span data-stu-id="01290-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="01290-103">Vyskytli sa problémy s blokovania eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="01290-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="01290-104">Tu je niekoľko najvhodnejších postupov na zváženie:</span><span class="sxs-lookup"><span data-stu-id="01290-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="01290-105">Skontrolujte stav zadržanej distribúcie.</span><span class="sxs-lookup"><span data-stu-id="01290-105">Check the hold distribution status.</span></span>  <span data-ttu-id="01290-106">Ak je stav **On (Pending) alebo Off** **(Pending) (Nevybavené),** počkajte, kým sa distribúcia zadržaho dokončí.</span><span class="sxs-lookup"><span data-stu-id="01290-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="01290-107">Zlúčenie vyhľadávania eDiscovery – zadržanie aktualizácií do jednej hromadnej požiadavky namiesto opakovaného aktualizovania politiky pre každú transakciu.</span><span class="sxs-lookup"><span data-stu-id="01290-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="01290-108">V Set-CaseHoldPolicy <policyname> Powershell Centra zabezpečenia a dodržiavania súladu spustite príkaz -RetryDistribution.</span><span class="sxs-lookup"><span data-stu-id="01290-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="01290-109">Podrobnosti nájdete v téme [Pripojenie zabezpečenia & Compliance Center PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="01290-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="01290-110">Kroky na kontrolu týchto nastavení a ďalšie osvedčené postupy na riešenie problémov s riešením blokovania eDiscovery nájdete v téme Riešenie chýb blokovania [eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="01290-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="01290-111">Informácie o riešení iných bežných problémov s eDiscovery nájdete v téme [Skúmanie, riešenie a riešenie bežných problémov s eDiscovery.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="01290-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
