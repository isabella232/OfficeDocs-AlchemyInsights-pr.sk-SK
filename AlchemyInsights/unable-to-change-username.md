---
title: Nie je možné zmeniť meno používateľa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440299"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="8df15-102">Nie je možné zmeniť meno používateľa</span><span class="sxs-lookup"><span data-stu-id="8df15-102">Unable to change UserName</span></span>

<span data-ttu-id="8df15-103">V niektorých prípadoch, UPN (UserPrincipalName) zmeny nie sú šírené do cloudu.</span><span class="sxs-lookup"><span data-stu-id="8df15-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="8df15-104">Chyby overenia sa môžu zobraziť na portáli služieb Office 365 alebo sa môžu zmeniť meno používateľa alebo e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="8df15-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="8df15-105">Ak chcete vyriešiť tento problém, manuálne nastaviť UserPrincipalName pomocou tohto príkazu prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8df15-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="8df15-106">**Príklad: Premenovanie používateľa**</span><span class="sxs-lookup"><span data-stu-id="8df15-106">**Example: Rename a user**</span></span>

<span data-ttu-id="8df15-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="8df15-107">PowerShellCopy</span></span>

<span data-ttu-id="8df15-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="8df15-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="8df15-109">Tento príkaz premenuje davidc@contoso.com na davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="8df15-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="8df15-110">Ďalšie informácie nájdete v téme [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="8df15-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>