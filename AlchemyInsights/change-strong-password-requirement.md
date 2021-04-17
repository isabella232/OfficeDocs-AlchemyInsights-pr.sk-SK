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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="753cd-102">Zmena strong password requirement</span><span class="sxs-lookup"><span data-stu-id="753cd-102">Change strong password requirement</span></span>

<span data-ttu-id="753cd-103">Spoločnosť Microsoft v predvolenom nastavení vyžaduje silné heslá.</span><span class="sxs-lookup"><span data-stu-id="753cd-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="753cd-104">Pomocou prostredia PowerShell môžete zakázať silné heslá pre konkrétnych používateľov pomocou týchto príkazov:</span><span class="sxs-lookup"><span data-stu-id="753cd-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="753cd-105">Ak chcete zakázať silné heslá pre všetkých používateľov, použite:</span><span class="sxs-lookup"><span data-stu-id="753cd-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="753cd-106">Ďalšie informácie o politike hesiel</span><span class="sxs-lookup"><span data-stu-id="753cd-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="753cd-107">Pripojenie k službe Microsoft 365 pomocou prostredia PowerShell</span><span class="sxs-lookup"><span data-stu-id="753cd-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="753cd-108">Ďalšie informácie o príkazoch v prostredí PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="753cd-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
