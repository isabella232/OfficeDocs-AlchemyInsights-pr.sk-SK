---
title: Zmena požiadavky na silné heslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681887"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="eb961-102">Zmena požiadavky na silné heslo</span><span class="sxs-lookup"><span data-stu-id="eb961-102">Change strong password requirement</span></span>

<span data-ttu-id="eb961-103">Spoločnosť Microsoft vyžaduje na základe predvoleného nastavenia silné heslá.</span><span class="sxs-lookup"><span data-stu-id="eb961-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="eb961-104">Pomocou prostredia PowerShell môžete vypnúť silné heslá pre konkrétnych používateľov pomocou tohto príkazu:</span><span class="sxs-lookup"><span data-stu-id="eb961-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="eb961-105">*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $FALSE*</span><span class="sxs-lookup"><span data-stu-id="eb961-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="eb961-106">Ďalšie informácie o politike hesiel</span><span class="sxs-lookup"><span data-stu-id="eb961-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="eb961-107">Pripojenie k službe Microsoft 365 s prostredím PowerShell</span><span class="sxs-lookup"><span data-stu-id="eb961-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="eb961-108">Ďalšie informácie o príkazoch prostredia PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="eb961-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
