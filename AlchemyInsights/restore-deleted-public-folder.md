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
# <a name="restore-a-deleted-public-folder"></a>Obnovenie odstráneného verejného priečinka

**Obnovenie odstránených položiek z verejného priečinka**:

- Pozrite [si nemôžete obnoviť odstránené položky z non-mail verejný priečinok v programe Outlook 2016](https://aka.ms/pfrec).
 
**Obnovenie odstráneného verejného priečinka (ľubovoľného typu)**: 

- Použite prosím nasledujúce EXO PowerShell príkaz:

    Syntax:

    >$pf = získať-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Názov-EQ "\<name_of_deleted_public_Folder"}; Súbor PublicFolder $pf. \<cesta identity cesty, kde sa obnoví priečinok>

    Príklad: nasledujúci príkaz obnoví Subfolder1 a umiestnite ho pod \Parent1:

    >$pf = získať-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Názov-EQ "Subfolder1"}; Súbor PublicFolder $pf. identita-Path \Parent1

Ďalšie podrobnosti nájdete [v časti Obnovenie odstráneného verejného priečinka](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
