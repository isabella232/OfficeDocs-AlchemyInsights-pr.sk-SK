---
title: Diagnostika problémov s prístupom k rôznym portom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030917"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika problémov s prístupom k rôznym portom

Ak chcete vyriešiť rôzne problémy s prístupom k portom, vykonajte tieto kroky:

1. Zastavte a vymiestníte virtuálny počítač (VM) z portálu, reštartujte VM a otestujte ho znova. 
2. Skontrolujte sieťové nastavenia VM a zistite, či máte skupiny zabezpečenia siete (NSG) blokujúce prenos. Môžete tiež použiť nástroj na overenie toku [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) adries pre sledovanie siete a skontrolovať, či nie sú k dispozícii NSG blokujúce prenosy, User-Defined trasy (UDRs) presmerovňovaním prenosu späť na lokálny prenos (predvolená trasa' 0.0.0.0/0) alebo na sieťové zariadenie.
Ak sa aj po vyskúšaní vyššie uvedených krokov vyskytnú problémy, zadajte názov VM a TCP port, na základe ktorých sa pokúšate odoslať poštu na ďalšie riešenie.

**Odporučené dokumenty**

[Obmedzenia a odporúčania pre odosielanie odchádzajúcich e-mailov cez port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)