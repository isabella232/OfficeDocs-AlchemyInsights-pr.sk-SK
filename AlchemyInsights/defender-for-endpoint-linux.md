---
title: Microsoft Defender pre Koncový bod v Linuxe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731980"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="2b659-102">Microsoft Defender pre Koncový bod v Linuxe</span><span class="sxs-lookup"><span data-stu-id="2b659-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="2b659-103">Podrobnú dokumentáciu k Linuxu nájdete [v téme Microsoft Defender pre koncový bod v Linuxe.](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux)</span><span class="sxs-lookup"><span data-stu-id="2b659-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="2b659-104">Informácie o systéme a inštalácii nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="2b659-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="2b659-105">Predpoklady</span><span class="sxs-lookup"><span data-stu-id="2b659-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="2b659-106">Systémové požiadavky</span><span class="sxs-lookup"><span data-stu-id="2b659-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="2b659-107">Pokyny na inštaláciu</span><span class="sxs-lookup"><span data-stu-id="2b659-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="2b659-108">Sieťové pripojenia</span><span class="sxs-lookup"><span data-stu-id="2b659-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="2b659-109">Pokyny nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="2b659-109">For instructions, see:</span></span>

- [<span data-ttu-id="2b659-110">Konfigurácia nastavenia servera proxy zariadenia a internetového pripojenia</span><span class="sxs-lookup"><span data-stu-id="2b659-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="2b659-111">Nasadenie aktualizácií pre Microsoft Defender pre koncový bod v Linuxe</span><span class="sxs-lookup"><span data-stu-id="2b659-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="2b659-112">Konfigurácia aplikácie Microsoft Defender pre koncový bod v Linuxe</span><span class="sxs-lookup"><span data-stu-id="2b659-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="2b659-113">Podporované príkazy</span><span class="sxs-lookup"><span data-stu-id="2b659-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="2b659-114">Potrebujem pomoc.</span><span class="sxs-lookup"><span data-stu-id="2b659-114">I need help!</span></span>

<span data-ttu-id="2b659-115">Ak nemôžete nájsť hľadané informácie/Pomocníka, spresnite hľadaný reťazec.</span><span class="sxs-lookup"><span data-stu-id="2b659-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="2b659-116">Pred kontaktním podpory spoločnosti Microsoft nezabudnite zhromaždiť údaje potrebné na to, aby ste problém preskúmali, a priložte ich k lístku.</span><span class="sxs-lookup"><span data-stu-id="2b659-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="2b659-117">Postup na zhromaždenie diagnostických informácií nájdete v téme Zhromažďovanie [diagnostických údajov.](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="2b659-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>