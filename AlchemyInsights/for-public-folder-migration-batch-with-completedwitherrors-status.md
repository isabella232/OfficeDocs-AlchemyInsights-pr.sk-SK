---
title: Pre verejný priečinok migrácie dávky s CompletedWithErrors stav
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158635"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pre verejný priečinok migrácie dávky s CompletedWithErrors stav

Použite nasledovný postup na dokončenie dávky, vynechanie veľké/zlé položky: 
1. Schváliť vynechané položky v dávke migrácie:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Ak chcete schváliť vynechané položky v žiadostiach o migráciu, ktoré sú "synchronizované", ale nie sú dokončené, použite nasledovný príkaz:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Dávka migrácie a žiadosti by mali pokračovať a dokončiť v priebehu niekoľkých minút.

