---
title: Nie je možné získať prístup k verejným priečinkom
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
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341418"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook sa nemôže pripojiť k verejným priečinkom

Ak prístup k verejným priečinkom nefunguje pre niektorých používateľov, vyskúšajte tento postup:

Pripojte sa k EXO PowerShell a nakonfigurujte parameter DefaultPublicFolderMailbox v používateľskom konte problém tak, aby zodpovedal parametru v pracovnom používateľskom konte.

Napríklad

Prístup k poštovej schránke WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Nastavenie poštovej schránky ProblemUser – DefaultPublicFolderMailbox \<value from previous command>

Počkajte aspoň jednu hodinu, kým sa zmena prejaví.

Ak problém pretrváva, použite [Tento postup](https://aka.ms/pfcte) na riešenie problémov s prístupom k verejným priečinkom pomocou Outlooku.
 
**Ak chcete určiť, ktorí používatelia majú prístup k verejným priečinkom pomocou Outlooku**:

1.  Použitie súpravy Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True alebo $FALSE  
      
    $true: povolenie prístupu používateľov k verejným priečinkom v Outlooku  
      
    $false: zabránenie prístupu používateľov k verejným priečinkom v Outlooku. Táto hodnota je predvolená.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Poznámka:** Tento postup umožňuje ovládať pripojenia iba pomocou počítačovej aplikácie Outlook pre klientov Windowsu. Používateľ môže pokračovať v prístupe k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.
 
Ďalšie informácie nájdete v téme [oznámenie podpory spravovaných pripojení k verejným priečinkom v Outlooku](https://aka.ms/controlpf).