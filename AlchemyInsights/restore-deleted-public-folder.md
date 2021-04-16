---
title: Obnovenie odstráneného verejného priečinka
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809454"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovenie odstráneného verejného priečinka

**Obnovenie odstránených položiek z verejného priečinka:**

- Pozrite si časť Odstránené položky z ne-mailového verejného priečinka [v Outlooku 2016](https://aka.ms/pfrec)nie je možné obnoviť.
 
**Obnovenie odstráneného verejného priečinka (ľubovoľného typu):** 

- Použite nasledujúci príkaz prostredia PowerShell EXO:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Príklad: Nasledujúci príkaz obnoví podpriečinok1 a umiestni ho do priečinka \Nadradený1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Ďalšie [podrobnosti nájdete v téme Obnovenie](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) odstráneného verejného priečinka.
