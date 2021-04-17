---
title: Nie je možné získať prístup k verejným priečinkom
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819527"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook sa nemôže pripojiť k verejným priečinkom

Ak prístup do verejného priečinka nefunguje pre niektorých používateľov, vyskúšajte tento postup:

Pripojte sa k exo PowerShell a nakonfigurujte parameter DefaultPublicFolderMailbox v problémovom používateľskom konte tak, aby zodpovedal parametru v pracovnom používateľskom konte.

Príklad:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Počkajte aspoň jednu hodinu, kým sa zmena prejaví.

Ak problém pretrváva, postupujte podľa tohto [postupu na riešenie problémov](https://aka.ms/pfcte) s prístupom do verejného priečinka pomocou Outlooku.
 
**Riadenie prístupu používateľov k verejným priečinkom pomocou Outlooku:**

1.  Použitie Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true alebo $false  
      
    $true: Povolenie prístupu používateľov k verejným priečinkom v Outlooku  
      
    $false: Zabránenie prístupu používateľov k verejným priečinkom v Outlooku. Táto hodnota je predvolená.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Poznámka** Týmto postupom môžete ovládať pripojenia iba k počítačovej aplikácii Outlook pre klientov s Windowsom. Používateľ môže aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.
 
Ďalšie informácie nájdete v téme [Oznámenie podpory kontrolovaných pripojení k verejným priečinkom v Outlooku.](https://aka.ms/controlpf)