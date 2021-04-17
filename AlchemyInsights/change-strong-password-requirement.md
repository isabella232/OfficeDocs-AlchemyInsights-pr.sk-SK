---
title: Zmena požiadavku na silné heslo
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818483"
---
# <a name="change-strong-password-requirement"></a>Zmena strong password requirement

Spoločnosť Microsoft v predvolenom nastavení vyžaduje silné heslá.

Pomocou prostredia PowerShell môžete zakázať silné heslá pre konkrétnych používateľov pomocou týchto príkazov:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Ak chcete zakázať silné heslá pre všetkých používateľov, použite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Ďalšie informácie o politike hesiel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Pripojenie k službe Microsoft 365 pomocou prostredia PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Ďalšie informácie o príkazoch v prostredí PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
