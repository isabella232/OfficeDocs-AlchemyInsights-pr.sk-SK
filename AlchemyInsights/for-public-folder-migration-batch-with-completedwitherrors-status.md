---
title: Dávka migrácie verejného priečinka so stavom CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744128"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Dávka migrácie verejného priečinka so stavom CompletedWithErrors

Na vyplnenie dávky použite nasledujúce kroky, ktoré vynechávajú veľké alebo zlé položky: 
1. Schváliť vynechané položky v dávke migrácie:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Na schválenie vynechaných položiek v požiadavkách na migráciu, ktoré sú synchronizované, ale nie sú dokončené, použite nasledujúci príkaz:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Dávka migrácie a žiadosti by sa mali obnoviť a vykonať v priebehu niekoľkých minút.

