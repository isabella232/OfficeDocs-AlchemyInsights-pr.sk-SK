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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996645"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook sa nemôže pripojiť k verejným priečinkom

Ak prístup do verejného priečinka nefunguje pre niektorých používateľov, vyskúšajte tento postup:

Pripojenie na EXO PowerShell a nakonfigurujte parameter DefaultPublicFolderMailbox v problémovom používateľskom konte tak, aby zodpovedal parametru v pracovnom používateľskom konte.

Príklad:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Počkajte aspoň jednu hodinu, kým sa zmena prejaví.

Ak problém pretrváva, postupujte podľa tohto [postupu na riešenie problémov](https://aka.ms/pfcte) s prístupom do verejného priečinka pomocou Outlook.
 
**Ovládanie prístupu používateľov k verejným priečinkom pomocou Outlook:**

1.  Použitie Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true alebo $false  
      
    $true: Povolenie prístupu používateľov k verejným priečinkom v Outlook  
      
    $false: Zabránenie prístupu používateľov k verejným priečinkom v Outlook. Táto hodnota je predvolená.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Poznámka** Týmto postupom môžete ovládať pripojenia iba s počítačovou Outlook pre Windows klientov. Používateľ môže aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlook pre Mac.
 
Ďalšie informácie nájdete v téme [Predstavenie podpory kontrolovaných pripojení k verejným priečinkom v Outlook.](https://aka.ms/controlpf)