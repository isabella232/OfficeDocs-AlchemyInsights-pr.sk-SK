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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043617"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pre verejný priečinok migrácie dávky s CompletedWithErrors stav

Použite nasledovný postup na dokončenie dávky, vynechanie veľké/zlé položky: 
1. Schváliť vynechané položky v dávke migrácie:

    Súbor Migrationdávkové \<batchname> Schvaľeskippeditems 
2. Ak chcete schváliť vynechané položky v žiadostiach o migráciu, ktoré sú "synchronizované", ale nie sú dokončené, použite nasledovný príkaz:

    $pf = získať-PublicFolderMailboxMigrationRequest | Získajte PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i v $pf) {if ($i. LargeItemsEncountered-gt 0 alebo $i. BadItemsEncountered-gt 0) {súbor PublicFolderMailboxMigrationRequest $i. identity. IdentifyingGuid-Skippeditemschvaľaltime $ ([dátum a čas]:: UtcNow)}}
3. Dávka migrácie a žiadosti by mali pokračovať a dokončiť v priebehu niekoľkých minút.

