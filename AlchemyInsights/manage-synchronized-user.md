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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie je možné nastaviť primárnu e-mailovú adresu, zmeniť atribúty používateľa alebo odstrániť alebo odstrániť synchronizovaného používateľa

Ak je zapnutá Synchronizácia adresárov pre vaše prostredie, niektoré atribúty používateľa alebo objektu nie je možné zmeniť pomocou Microsoft 365 admin Center.

Plne spravovať synchronizované používateľov a všetky ich atribúty, použite miestne Active Directory Users a skupiny Management Console (Adsiedit. msc).  

Prípadne môžete zmeniť jednotlivých používateľov alebo atribúty pre synchronizovaných používateľov pomocou prostredia PowerShell, ako je uvedené v týchto bežných príkladoch: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
