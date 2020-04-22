---
title: Zmeniť silnú požiadavku na heslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706576"
---
# <a name="change-strong-password-requirement"></a>Zmeniť silnú požiadavku na heslo

Spoločnosť Microsoft vyžaduje predvolene silné heslá. 

Pomocou prostredia PowerShell môžete vypnúť silné heslá pre konkrétnych používateľov pomocou tohto príkazu:<br>
*Súbor MsolUser – UserPrincipalName <UserPrincipalName> – strongpasswordrequired $FALSE*

- [Ďalšie informácie o politike hesiel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Ako sa pripojiť k Microsoft 365 s PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Ďalšie informácie o PowerShell MsolUser príkazy](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
