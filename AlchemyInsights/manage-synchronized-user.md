---
title: Spravovať synchronizovaného používateľa
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542018"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="04a84-102">Nedá sa nastaviť primárnu e-mailovú adresu alebo zmeniť používateľské atribúty</span><span class="sxs-lookup"><span data-stu-id="04a84-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="04a84-103">Ak Synchronizácia adresárov je povolené pre vaše prostredie, niektoré atribúty používateľa alebo objektu nie je možné zmeniť pomocou Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="04a84-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="04a84-104">Plne Spravovať synchronizáciu používateľov a všetky ich atribúty, použitie lokálnej služby active directory používatelia a skupiny riadenia konzoly (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="04a84-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="04a84-105">Prípadne môžete jednotlivým používateľom alebo atribúty pre synchronizáciu používateľov pomocou powershell, ako je uvedené v týchto bežných príkladoch:</span><span class="sxs-lookup"><span data-stu-id="04a84-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="04a84-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="04a84-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="04a84-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test používateľa" - priezvisko "User"-názov "Manager"-oddelenie "HR"</span><span class="sxs-lookup"><span data-stu-id="04a84-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="04a84-108">Odstránenie MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="04a84-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>