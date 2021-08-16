---
title: Riadenie prístupu k verejným priečinkom pomocou Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032573"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Riadenie prístupu k verejným priečinkom pomocou Outlook

Ovládanie prístupu používateľov k verejným priečinkom pomocou Outlook:

1. Použite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Povolenie prístupu používateľov k verejným priečinkom v Outlook  
$false: Zabránenie prístupu používateľov k verejným priečinkom v Outlook. Táto hodnota je predvolená.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Poznámka: Tento postup dokáže ovládať iba pripojenia k počítačovej Outlook pre Windows klientov. Používatelia môžu aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlook pre Mac.

Ďalšie informácie nájdete v téme [Riadené pripojenia k verejným priečinkom Outlook](https://aka.ms/controlpf) ďalšie informácie.
