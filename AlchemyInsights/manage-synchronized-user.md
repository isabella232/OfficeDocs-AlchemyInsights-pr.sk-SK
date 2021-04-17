---
title: Spravovať synchronizovaných používateľov
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823982"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="5f866-102">Nie je možné nastaviť primárnu e-mailovú adresu, zmeniť atribúty používateľa alebo odstrániť synchronizovaného používateľa</span><span class="sxs-lookup"><span data-stu-id="5f866-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="5f866-103">Ak je pre vaše prostredie povolená synchronizácia adresárov, niektoré atribúty používateľov alebo objektov nie je možné zmeniť pomocou Centra spravovania služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5f866-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="5f866-104">Ak chcete plne spravovať synchronizovaných používateľov a všetky ich atribúty, použite lokálnu konzolu správy služby Active Directory (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="5f866-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="5f866-105">Prípadne môžete zmeniť jednotlivých používateľov alebo atribúty synchronizovaných používateľov pomocou prostredia PowerShell, ako je to znázornené v týchto bežných príkladoch:</span><span class="sxs-lookup"><span data-stu-id="5f866-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
