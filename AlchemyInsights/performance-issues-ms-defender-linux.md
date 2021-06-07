---
title: Problémy s výkonom aplikácie Microsoft Defender pre koncový bod v Linuxe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794228"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="96ca3-102">Problémy s výkonom aplikácie Microsoft Defender pre koncový bod v Linuxe</span><span class="sxs-lookup"><span data-stu-id="96ca3-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="96ca3-103">Tento článok vás prevedie krokmi, ktoré sú potrebné na identifikáciu problémov s výkonom v aplikácii Microsoft Defender pre koncový bod v Linuxe.</span><span class="sxs-lookup"><span data-stu-id="96ca3-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="96ca3-104">Je dôležité najprv overiť, či sa problém vyriešil s najnovšou [verziou.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="96ca3-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="96ca3-105">Ak chcete začať skúmanie, pozrite si [tému Riešenie problémov s výkonom aplikácie Microsoft Defender pre koncový bod v Linuxe.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="96ca3-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="96ca3-106">Vylúčenia</span><span class="sxs-lookup"><span data-stu-id="96ca3-106">Exclusions</span></span>

<span data-ttu-id="96ca3-107">Vylúčenia môžu pomôcť obmedziť problémy s výkonom.</span><span class="sxs-lookup"><span data-stu-id="96ca3-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="96ca3-108">Skôr než začnete, skontrolujte svoje vylúčenia, aby ste ďalšie riziko vedeli a zdokumentovali.</span><span class="sxs-lookup"><span data-stu-id="96ca3-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="96ca3-109">Ďalšie informácie nájdete v téme [Konfigurácia a overenie vylúčení pre Microsoft Defender pre koncový bod v Linuxe.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="96ca3-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="96ca3-110">Ak máte viacero súborov, & chcete vylúčiť a všetky sa nachádzajú v tom istom prípojkovom bodu, pravdepodobne bude jednoduchšie vylúčiť prípojný bod.</span><span class="sxs-lookup"><span data-stu-id="96ca3-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="96ca3-111">Od februára vydanie 101.22.80 môžete vylúčiť celý bod pripojenia.</span><span class="sxs-lookup"><span data-stu-id="96ca3-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="96ca3-112">Ak je napríklad /mnt/backup mountpoint, môžete do zoznamu vylúčiť pridať príkaz /mnt/backup spustením tohto príkazu:</span><span class="sxs-lookup"><span data-stu-id="96ca3-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="96ca3-113">**Poznámka:** Pridanie vylúčenia zvyšuje riziko, že sa nenájsť malvér nenáli, a mali by sa spracovávať a implementovať opatrne.</span><span class="sxs-lookup"><span data-stu-id="96ca3-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="96ca3-114">Potrebujete pomoc?</span><span class="sxs-lookup"><span data-stu-id="96ca3-114">Need Help?</span></span>

<span data-ttu-id="96ca3-115">Aby sme vám pomohli najefektívnejším spôsobom, pred otvorením prípadu podpory zhromaždite diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="96ca3-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
