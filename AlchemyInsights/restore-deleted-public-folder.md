---
title: Obnovenie odstráneného verejného priečinka
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774546"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovenie odstráneného verejného priečinka

**Obnovenie odstránených položiek z verejného priečinka**:

- Pozrite si tému [nie je možné obnoviť odstránené položky z nepoštového verejného priečinka v outlooku 2016](https://aka.ms/pfrec).
 
**Obnovenie odstráneného verejného priečinka (ľubovoľného typu)**: 

- Použite nasledujúci príkaz EXO PowerShell:

    Syntax

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Príklad: nasledujúci príkaz obnoví Subfolder1 a umiestni ho pod \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Ďalšie informácie nájdete v téme [Obnovenie odstráneného verejného priečinka](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
