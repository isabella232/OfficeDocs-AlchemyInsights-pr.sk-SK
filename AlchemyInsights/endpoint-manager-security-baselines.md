---
title: EndPoint Manager – pôvodné hodnoty zabezpečenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421090"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="26a8e-102">EndPoint Manager – pôvodné hodnoty zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="26a8e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="26a8e-103">Pôvodné hodnoty zabezpečenia sú vopred nakonfigurované skupiny nastavení Windowsu, ktoré vám pomôžu použiť nastavenia zabezpečenia odporúčané príslušnými tímami zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="26a8e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="26a8e-104">Tieto pôvodné hodnoty je možné prispôsobiť tak, aby sa doručovali iba požadované nastavenia a hodnoty.</span><span class="sxs-lookup"><span data-stu-id="26a8e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="26a8e-105">Ďalšie informácie o pôvodných plánoch zabezpečenia nájdete v téme [Použitie pôvodných bodov zabezpečenia na konfiguráciu zariadení s Windowsom 10 v intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="26a8e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="26a8e-106">Pre tieto produkty v súčasnosti existujú pôvodné hodnoty:</span><span class="sxs-lookup"><span data-stu-id="26a8e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="26a8e-107">Nastavenia zabezpečenia MDM systému Windows</span><span class="sxs-lookup"><span data-stu-id="26a8e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="26a8e-108">Zabezpečenie aplikácie Microsoft Defender pre EndPoint</span><span class="sxs-lookup"><span data-stu-id="26a8e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="26a8e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="26a8e-109">Microsoft Edge</span></span>

<span data-ttu-id="26a8e-110">Všetky pôvodné hodnoty sa pravidelne aktualizujú a uvoľňujú v prírastkových verziách.</span><span class="sxs-lookup"><span data-stu-id="26a8e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="26a8e-111">Každá verzia pridá alebo odstráni nastavenia z predchádzajúcej verzie, aby sa zabezpečilo, že základná čiara spĺňa aktuálne pokyny.</span><span class="sxs-lookup"><span data-stu-id="26a8e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="26a8e-112">Konzola s pôvodnými plánmi zabezpečenia v časti Zabezpečenie koncového bodu umožňuje porovnanie rôznych verzií tak, že zmeny z verzie na verziu sa zobrazia.</span><span class="sxs-lookup"><span data-stu-id="26a8e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="26a8e-113">Pokyny na najefektívnejšie zmeny toho, ktorá verzia pôvodného plánu je nasadená, nájdete v téme Správa profilov pôvodného plánu zabezpečenia [v Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="26a8e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="26a8e-114">Po nasadení základnej hodnoty zabezpečenia môžete sledovať stav nasadenia a skontrolovať nastavenia na každom zariadení.</span><span class="sxs-lookup"><span data-stu-id="26a8e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="26a8e-115">**Poznámka:** Vykazovanie údajov pre pôvodné hodnoty môže trvať až 24 hodín, kým sa zobrazia od prvého nasadenia do zariadenia, a až 6 hodín pre ďalšie aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="26a8e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="26a8e-116">Najčastejšou príčinou, prečo sa nastavenie pôvodného plánu nepoužíva, je to, že rovnaké nastavenie sa používa v inom profile.</span><span class="sxs-lookup"><span data-stu-id="26a8e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="26a8e-117">Tento scenár môžete preskúmať pre konkrétne zariadenie tak, že toto zariadenie vyberiete z uzla Stav zariadenia v profile Plán zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="26a8e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="26a8e-118">Podrobnosti nájdete v téme [Riešenie konfliktov pre pôvodné hodnoty zabezpečenia.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="26a8e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>