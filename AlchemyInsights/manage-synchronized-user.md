---
title: Správa synchronizovaného používateľa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407365"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="10fdc-102">Nie je možné nastaviť primárnu e-mailovú adresu, zmeniť atribúty používateľa alebo odstrániť alebo odstrániť synchronizovaného používateľa</span><span class="sxs-lookup"><span data-stu-id="10fdc-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="10fdc-103">Ak je zapnutá Synchronizácia adresárov pre vaše prostredie, niektoré atribúty používateľa alebo objektu nie je možné zmeniť pomocou Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="10fdc-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="10fdc-104">Plne spravovať synchronizované používateľov a všetky ich atribúty, použite miestne Active Directory Users a skupiny Management Console (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="10fdc-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="10fdc-105">Prípadne môžete zmeniť jednotlivých používateľov alebo atribúty pre synchronizovaných používateľov pomocou prostredia PowerShell, ako je uvedené v týchto bežných príkladoch:</span><span class="sxs-lookup"><span data-stu-id="10fdc-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
