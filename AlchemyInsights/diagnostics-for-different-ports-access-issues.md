---
title: Diagnostika pre rôzne problémy s prístupom k portom
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036809"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika pre rôzne problémy s prístupom k portom

Ak chcete vyriešiť rôzne problémy s prístupom k portu, vykonajte tieto kroky:

1. Zastavte alebo oddeľte virtuálny počítač (VM) z portálu, reštartujte VM a otestujte znova. 
2. Skontrolujte nastavenia siete VM a zistite, či máte zablokované prenosy v skupinách zabezpečenia siete (NSGs). Môžete tiež použiť [nástroj na overenie toku IP nástroja Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) na kontrolu NSGs blokovania premávky, User-Defined trás (UDRs) presmeruje prenos späť na lokálne (' predvolená trasa ' 0.0.0.0/0) alebo do sieťového zariadenia.
Ak sa vyskytnú problémy aj po vyskúšaní vyššie uvedených krokov, zadajte názov VM a port TCP, ku ktorému sa pokúšate odoslať poštu na ďalšiu diagnózu.

**Odporučené dokumenty**

[Obmedzenia a odporúčania na odosielanie odchádzajúcich e-mailov cez port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)