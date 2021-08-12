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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943390"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovenie odstráneného verejného priečinka

**Obnovenie odstránených položiek z verejného priečinka:**

- Pozrite [si časť Odstránené položky z ne-mailového](https://aka.ms/pfrec)verejného priečinka nie je možné obnoviť v Outlook 2016.
 
**Obnovenie odstráneného verejného priečinka (ľubovoľného typu):** 

- Použite nasledujúci príkaz prostredia PowerShell EXO:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Príklad: Nasledujúci príkaz obnoví podpriečinok1 a umiestni ho do priečinka \Nadradený1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Ďalšie [podrobnosti nájdete v téme Obnovenie](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) odstráneného verejného priečinka.
