---
title: Defender Endpoint check sensor status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676337"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="d9e7d-102">Defender Endpoint check sensor status</span><span class="sxs-lookup"><span data-stu-id="d9e7d-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="d9e7d-103">Dlaždica **Zariadenia s problémami senzora** sa nachádza na tabuli Operácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="d9e7d-104">Táto dlaždica poskytuje informácie o schopnosti jednotlivých zariadení poskytovať údaje senzora a komunikovať so službu Defender pre koncový bod.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="d9e7d-105">V tejto matici sa nachádza hlásenie, koľko zariadení vyžaduje pozornosť, a pomáha identifikovať problematické zariadenia a prijať opatrenia na odstránenie známych problémov.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="d9e7d-106">Dva indikátory stavu na dlaždici poskytujú informácie o počte zariadení, ktoré sa službe nesprávne nahlasujú:</span><span class="sxs-lookup"><span data-stu-id="d9e7d-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="d9e7d-107">**Nesprávne nakonfigurované** Zariadenia, ktoré môžu čiastočne vykazovať údaje senzora do služby Defender pre koncové body a môžu mať chyby konfigurácie, ktoré je potrebné opraviť.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="d9e7d-108">**Neaktívne** Zariadenia, ktoré zastavili vykazovanie do služby Defender for Endpoint na viac ako sedem dní v priebehu minulého mesiaca.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="d9e7d-109">Po kliknutí na niektorú zo skupín sa nasmeruje na zoznam Zariadenia filtrovaný podľa vašich možností.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="d9e7d-110">V zozname Zariadenia môžete zoznam stavov filtrovať podľa tohto stavu:</span><span class="sxs-lookup"><span data-stu-id="d9e7d-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="d9e7d-111">**Aktívne** Zariadenia, ktoré aktívne hlásia službu Defender pre koncový bod.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="d9e7d-112">**Nesprávne nakonfigurované** Zariadenia, ktoré môžu čiastočne vykazovať údaje senzora do služby Defender pre koncový bod, ale majú chyby konfigurácie, ktoré je potrebné opraviť.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="d9e7d-113">Nesprávne nakonfigurované zariadenia môžu mať jeden alebo kombináciu nasledujúcich problémov:</span><span class="sxs-lookup"><span data-stu-id="d9e7d-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="d9e7d-114">Žiadne údaje senzora – zariadenia prestali odosielať údaje senzora.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="d9e7d-115">Zo zariadenia možno spustiť obmedzené upozornenia.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="d9e7d-116">Komunikácia s poruchou – možnosť komunikácie so zariadením je s poruchou.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="d9e7d-117">Odosielanie súborov na podrobnú analýzu, blokovanie súborov, izolovanie zariadení od siete a ďalšie akcie, ktoré vyžadujú komunikáciu so zariadením, nemusia fungovať.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="d9e7d-118">**Neaktívne** Zariadenia, ktoré prestali vykazovať službu Defender pre koncový bod.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="d9e7d-119">Celý zoznam vo formáte CSV môžete stiahnuť pomocou funkcie Exportovať.</span><span class="sxs-lookup"><span data-stu-id="d9e7d-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="d9e7d-120">Ďalšie informácie nájdete v téme [Kontrola stavu senzora v aplikácii Microsoft Defender pre koncový bod.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="d9e7d-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="d9e7d-121">Ďalšie informácie o tom, čo spôsobilo neaktívne alebo nesprávne nakonfigurované zariadenie, nájdete v téme Oprava nevhodných senzorov v [aplikácii Microsoft Defender pre koncový bod.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="d9e7d-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
