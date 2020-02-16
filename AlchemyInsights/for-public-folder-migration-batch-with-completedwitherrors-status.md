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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="16e02-102">Pre verejný priečinok migrácie dávky s CompletedWithErrors stav</span><span class="sxs-lookup"><span data-stu-id="16e02-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="16e02-103">Použite nasledovný postup na dokončenie dávky, vynechanie veľké/zlé položky:</span><span class="sxs-lookup"><span data-stu-id="16e02-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="16e02-104">Schváliť vynechané položky v dávke migrácie:</span><span class="sxs-lookup"><span data-stu-id="16e02-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="16e02-105">Súbor Migrationdávkové \<batchname> Schvaľeskippeditems</span><span class="sxs-lookup"><span data-stu-id="16e02-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="16e02-106">Ak chcete schváliť vynechané položky v žiadostiach o migráciu, ktoré sú "synchronizované", ale nie sú dokončené, použite nasledovný príkaz:</span><span class="sxs-lookup"><span data-stu-id="16e02-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="16e02-107">$pf = získať-PublicFolderMailboxMigrationRequest | Získajte PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i v $pf) {if ($i. LargeItemsEncountered-gt 0 alebo $i. BadItemsEncountered-gt 0) {súbor PublicFolderMailboxMigrationRequest $i. identity. IdentifyingGuid-Skippeditemschvaľaltime $ ([dátum a čas]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="16e02-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="16e02-108">Dávka migrácie a žiadosti by mali pokračovať a dokončiť v priebehu niekoľkých minút.</span><span class="sxs-lookup"><span data-stu-id="16e02-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

