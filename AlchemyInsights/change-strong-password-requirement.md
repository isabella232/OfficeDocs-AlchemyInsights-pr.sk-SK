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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="77068-102">Zmeniť silnú požiadavku na heslo</span><span class="sxs-lookup"><span data-stu-id="77068-102">Change strong password requirement</span></span>

<span data-ttu-id="77068-103">Spoločnosť Microsoft vyžaduje predvolene silné heslá.</span><span class="sxs-lookup"><span data-stu-id="77068-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="77068-104">Pomocou prostredia PowerShell môžete vypnúť silné heslá pre konkrétnych používateľov pomocou tohto príkazu:</span><span class="sxs-lookup"><span data-stu-id="77068-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="77068-105">*Súbor MsolUser – UserPrincipalName <UserPrincipalName> – strongpasswordrequired $FALSE*</span><span class="sxs-lookup"><span data-stu-id="77068-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="77068-106">Ďalšie informácie o politike hesiel</span><span class="sxs-lookup"><span data-stu-id="77068-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="77068-107">Ako sa pripojiť k balíku Office 365 s PowerShell</span><span class="sxs-lookup"><span data-stu-id="77068-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="77068-108">Ďalšie informácie o PowerShell MsolUser príkazy</span><span class="sxs-lookup"><span data-stu-id="77068-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="77068-109">Nastavenie hesla individuálneho používateľa na nikdy neskončí</span><span class="sxs-lookup"><span data-stu-id="77068-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
