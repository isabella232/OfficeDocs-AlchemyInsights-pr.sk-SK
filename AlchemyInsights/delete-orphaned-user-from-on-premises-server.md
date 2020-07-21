---
title: Odstránenie osamoteného používateľa z lokálneho servera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198588"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="4fdf1-102">Odstránenie osamoteného používateľa z lokálneho servera</span><span class="sxs-lookup"><span data-stu-id="4fdf1-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="4fdf1-103">Ak chcete odstrániť osamoteného používateľa, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="4fdf1-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="4fdf1-104">Vynútiť synchronizáciu adresárov podľa pokynov v časti [Čo je hybridná identita služby Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="4fdf1-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="4fdf1-105">Ak chcete overiť synchronizáciu adresárov, pozrite si [tému Čo je hybridná identita služby Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="4fdf1-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="4fdf1-106">Ak synchronizácia funguje správne, ale odstránenie objektu služby Active Directory nerozšíri Azure AD, manuálne odstrániť osamotený objekt pomocou jedného z nasledujúcich Azure Active Directory modul pre rutiny cmdlet prostredia Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4fdf1-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="4fdf1-107">Odstrániť MsolContact</span><span class="sxs-lookup"><span data-stu-id="4fdf1-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="4fdf1-108">Odstrániť MsolGroup</span><span class="sxs-lookup"><span data-stu-id="4fdf1-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="4fdf1-109">Odstrániť MsolUser</span><span class="sxs-lookup"><span data-stu-id="4fdf1-109">Remove-MsolUser</span></span>

    <span data-ttu-id="4fdf1-110">Ak napríklad chcete odstrániť osamotený john.smith@contoso.com identifikácie používateľa, pôvodne vytvorený pomocou synchronizácie adresárov, spustite rutinu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="4fdf1-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="4fdf1-111">Odstrániť MsolUser-UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="4fdf1-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>