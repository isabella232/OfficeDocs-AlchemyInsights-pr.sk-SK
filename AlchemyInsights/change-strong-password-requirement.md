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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286293"
---
# <a name="change-strong-password-requirement"></a>Zmeniť silnú požiadavku na heslo

Spoločnosť Microsoft vyžaduje predvolene silné heslá. 

Pomocou prostredia PowerShell môžete vypnúť silné heslá pre konkrétnych používateľov pomocou tohto príkazu:<br>
*Súbor MsolUser – UserPrincipalName <UserPrincipalName> – strongpasswordrequired $FALSE*

- [Ďalšie informácie o politike hesiel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Ako sa pripojiť k balíku Office 365 s PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Ďalšie informácie o PowerShell MsolUser príkazy](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Nastavenie hesla individuálneho používateľa na nikdy neskončí](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
