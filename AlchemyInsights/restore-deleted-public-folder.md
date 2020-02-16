---
title: Obnovenie odstráneného verejného priečinka
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063742"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="649c3-102">Obnovenie odstráneného verejného priečinka</span><span class="sxs-lookup"><span data-stu-id="649c3-102">Restore a deleted public folder</span></span>

<span data-ttu-id="649c3-103">**Obnovenie odstránených položiek z verejného priečinka**:</span><span class="sxs-lookup"><span data-stu-id="649c3-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="649c3-104">Pozrite [si nemôžete obnoviť odstránené položky z non-mail verejný priečinok v programe Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="649c3-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="649c3-105">**Obnovenie odstráneného verejného priečinka (ľubovoľného typu)**:</span><span class="sxs-lookup"><span data-stu-id="649c3-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="649c3-106">Použite prosím nasledujúce EXO PowerShell príkaz:</span><span class="sxs-lookup"><span data-stu-id="649c3-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="649c3-107">Syntax:</span><span class="sxs-lookup"><span data-stu-id="649c3-107">Syntax:</span></span>

    ><span data-ttu-id="649c3-108">$pf = získať-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Názov-EQ "\<name_of_deleted_public_Folder"}; Súbor PublicFolder $pf. \<cesta identity cesty, kde sa obnoví priečinok></span><span class="sxs-lookup"><span data-stu-id="649c3-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="649c3-109">Príklad: nasledujúci príkaz obnoví Subfolder1 a umiestnite ho pod \Parent1:</span><span class="sxs-lookup"><span data-stu-id="649c3-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="649c3-110">$pf = získať-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Názov-EQ "Subfolder1"}; Súbor PublicFolder $pf. identita-Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="649c3-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="649c3-111">Ďalšie podrobnosti nájdete [v časti Obnovenie odstráneného verejného priečinka](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="649c3-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
