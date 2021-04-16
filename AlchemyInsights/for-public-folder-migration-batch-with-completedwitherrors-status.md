---
title: Pre dávku migrácie verejných priečinkov so stavom CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812479"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pre dávku migrácie verejných priečinkov so stavom CompletedWithErrors

Pomocou nasledujúcich krokov dokončite dávku a vynecháte veľké alebo zlé položky: 
1. Schválenie vynechaných položiek v dávke migrácie:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Na schválenie vynechaných položiek v žiadostiach o migráciu, ktoré sú synchronizované, ale nie sú dokončené, použite nasledujúci príkaz:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Dávka migrácie a žiadosti by sa mali obnoviť a dokončiť o niekoľko minút.

