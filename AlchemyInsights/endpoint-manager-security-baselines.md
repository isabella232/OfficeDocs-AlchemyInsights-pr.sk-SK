---
title: EndPoint Manager – základné úrovne zabezpečenia
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440908"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="129a9-102">EndPoint Manager – základné úrovne zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="129a9-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="129a9-103">Základné úrovne zabezpečenia sú vopred nakonfigurované skupiny nastavení Windowsu, ktoré vám pomôžu použiť nastavenia zabezpečenia odporúčané príslušnými bezpečnostnými tímami.</span><span class="sxs-lookup"><span data-stu-id="129a9-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="129a9-104">Tieto základné úrovne je možné prispôsobiť tak, aby obsahovali iba požadované nastavenia a hodnoty.</span><span class="sxs-lookup"><span data-stu-id="129a9-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="129a9-105">Ďalšie informácie o základných úrovniach zabezpečenia nájdete v téme [Použitie základných úrovní zabezpečenia na konfiguráciu zariadení s Windowsom 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="129a9-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="129a9-106">V súčasnosti existujú základné úrovne pre tieto produkty:</span><span class="sxs-lookup"><span data-stu-id="129a9-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="129a9-107">Nastavenie zabezpečenia MDM systému Windows</span><span class="sxs-lookup"><span data-stu-id="129a9-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="129a9-108">Zabezpečenie Microsoft Defender pre koncové body</span><span class="sxs-lookup"><span data-stu-id="129a9-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="129a9-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="129a9-109">Microsoft Edge</span></span>

<span data-ttu-id="129a9-110">Všetky základné úrovne sa pravidelne aktualizujú a vydávajú v prírastkových verziách.</span><span class="sxs-lookup"><span data-stu-id="129a9-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="129a9-111">V každej verzii sa pridávajú alebo odstraňujú nastavenia z predchádzajúcej verzie, aby sa zabezpečilo, že základná úroveň spĺňa aktuálne pokyny.</span><span class="sxs-lookup"><span data-stu-id="129a9-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="129a9-112">Konzola so základnými úrovňami zabezpečenia v Endpoint Security umožňuje porovnať rôzne verzie pomocou viditeľných zmien medzi verziami.</span><span class="sxs-lookup"><span data-stu-id="129a9-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="129a9-113">Pokyny na najefektívnejšiu zmenu nasadenej verzie základnej úrovne nájdete v téme [Spravovanie základných úrovní zabezpečenia v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="129a9-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="129a9-114">Po nasadení základnej úrovne zabezpečenia môžete monitorovať stav nasadenia a skontrolovať nastavenia podľa jednotlivých zariadení.</span><span class="sxs-lookup"><span data-stu-id="129a9-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="129a9-115">**Poznámka:** Údaje zostáv pre základné úrovne sa môžu zobraziť až o 24 hodín od počiatočného nasadenia do zariadenia a až o 6 hodín v prípade ďalších aktualizácií.</span><span class="sxs-lookup"><span data-stu-id="129a9-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="129a9-116">Najčastejšou príčinou nepoužitia nastavení základnej úrovne je to, že rovnaké nastavenie sa používa v inom profile.</span><span class="sxs-lookup"><span data-stu-id="129a9-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="129a9-117">Tento scenár možno preskúmať pre konkrétne zariadenie tak, že ho vyberiete z uzla stavu zariadenia v profile základnej úrovne zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="129a9-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="129a9-118">Podrobnosti nájdete v téme [Riešenie konfliktov základných úrovní zabezpečenia](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="129a9-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>