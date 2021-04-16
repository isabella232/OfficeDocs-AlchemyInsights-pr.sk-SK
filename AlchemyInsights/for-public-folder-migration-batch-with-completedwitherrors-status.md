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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="8b82b-102">Pre dávku migrácie verejných priečinkov so stavom CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="8b82b-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="8b82b-103">Pomocou nasledujúcich krokov dokončite dávku a vynecháte veľké alebo zlé položky:</span><span class="sxs-lookup"><span data-stu-id="8b82b-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="8b82b-104">Schválenie vynechaných položiek v dávke migrácie:</span><span class="sxs-lookup"><span data-stu-id="8b82b-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="8b82b-105">Na schválenie vynechaných položiek v žiadostiach o migráciu, ktoré sú synchronizované, ale nie sú dokončené, použite nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="8b82b-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="8b82b-106">Dávka migrácie a žiadosti by sa mali obnoviť a dokončiť o niekoľko minút.</span><span class="sxs-lookup"><span data-stu-id="8b82b-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

