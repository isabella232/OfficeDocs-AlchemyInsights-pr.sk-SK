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
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070699"
---
# <a name="change-strong-password-requirement"></a>Zmena strong password requirement

Spoločnosť Microsoft v predvolenom nastavení vyžaduje silné heslá.

Pomocou prostredia PowerShell môžete zakázať silné heslá pre konkrétnych používateľov pomocou týchto príkazov:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Ak chcete zakázať silné heslá pre všetkých používateľov, použite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Ďalšie informácie o politike hesiel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Pripojenie k E-Microsoft 365 pomocou prostredia PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Ďalšie informácie o príkazoch v prostredí PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
