---
title: Riadenie prístupu k verejným priečinkom pomocou Outlooku
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816755"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Riadenie prístupu k verejným priečinkom pomocou Outlooku

Riadenie prístupu používateľov k verejným priečinkom pomocou Outlooku:

1. Použite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Povolenie prístupu používateľov k verejným priečinkom v Outlooku  
$false: Zabránenie prístupu používateľov k verejným priečinkom v Outlooku. Táto hodnota je predvolená.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Poznámka: Tento postup dokáže ovládať iba pripojenia k počítačovej aplikácii Outlook pre klientov s Windowsom. Používatelia môžu aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.

Ďalšie informácie nájdete v téme [Riadené pripojenia k verejným priečinkom v Outlooku.](https://aka.ms/controlpf)
