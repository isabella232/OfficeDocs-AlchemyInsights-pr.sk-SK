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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="92fdf-102">Zmeniť silnú požiadavku na heslo</span><span class="sxs-lookup"><span data-stu-id="92fdf-102">Change strong password requirement</span></span>

<span data-ttu-id="92fdf-103">Spoločnosť Microsoft vyžaduje predvolene silné heslá.</span><span class="sxs-lookup"><span data-stu-id="92fdf-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="92fdf-104">Pomocou prostredia PowerShell môžete vypnúť silné heslá pre konkrétnych používateľov pomocou tohto príkazu:</span><span class="sxs-lookup"><span data-stu-id="92fdf-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="92fdf-105">*Súbor MsolUser – UserPrincipalName <UserPrincipalName> – strongpasswordrequired $FALSE*</span><span class="sxs-lookup"><span data-stu-id="92fdf-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="92fdf-106">Ďalšie informácie o politike hesiel</span><span class="sxs-lookup"><span data-stu-id="92fdf-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="92fdf-107">Ako sa pripojiť k Microsoft 365 s PowerShell</span><span class="sxs-lookup"><span data-stu-id="92fdf-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="92fdf-108">Ďalšie informácie o PowerShell MsolUser príkazy</span><span class="sxs-lookup"><span data-stu-id="92fdf-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
