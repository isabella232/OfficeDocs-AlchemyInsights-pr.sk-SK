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
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problémy s výkonom aplikácie Microsoft Defender pre koncový bod v Linuxe

Tento článok vás prevedie krokmi, ktoré sú potrebné na identifikáciu problémov s výkonom v aplikácii Microsoft Defender pre koncový bod v Linuxe.

Je dôležité najprv overiť, či sa problém vyriešil s najnovšou [verziou.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Ak chcete začať skúmanie, pozrite si [tému Riešenie problémov s výkonom aplikácie Microsoft Defender pre koncový bod v Linuxe.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Vylúčenia

Vylúčenia môžu pomôcť obmedziť problémy s výkonom. Skôr než začnete, skontrolujte svoje vylúčenia, aby ste ďalšie riziko vedeli a zdokumentovali.

Ďalšie informácie nájdete v téme [Konfigurácia a overenie vylúčení pre Microsoft Defender pre koncový bod v Linuxe.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Ak máte viacero súborov, & chcete vylúčiť a všetky sa nachádzajú v tom istom prípojkovom bodu, pravdepodobne bude jednoduchšie vylúčiť prípojný bod. Od februára vydanie 101.22.80 môžete vylúčiť celý bod pripojenia.

Ak je napríklad /mnt/backup mountpoint, môžete do zoznamu vylúčiť pridať príkaz /mnt/backup spustením tohto príkazu:

`$ mdatp exclusion folder add –path /mnt/backup`

**Poznámka:** Pridanie vylúčenia zvyšuje riziko, že sa nenájsť malvér nenáli, a mali by sa spracovávať a implementovať opatrne.

## <a name="need-help"></a>Potrebujete pomoc?

Aby sme vám pomohli najefektívnejším spôsobom, pred otvorením prípadu podpory zhromaždite diagnostické údaje.
