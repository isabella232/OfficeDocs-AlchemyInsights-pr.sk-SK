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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114793"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie je možné nastaviť primárnu e-mailovú adresu, zmeniť atribúty používateľa alebo odstrániť synchronizovaného používateľa

Ak je pre vaše prostredie povolená synchronizácia adresárov, niektoré atribúty používateľov alebo objektov nie je možné zmeniť pomocou Centrum spravovania služby Microsoft 365.

Ak chcete plne spravovať synchronizovaných používateľov a všetky ich atribúty, použite lokálnu konzolu správy služby Active Directory (adsiedit.msc).  

Prípadne môžete zmeniť jednotlivých používateľov alebo atribúty synchronizovaných používateľov pomocou prostredia PowerShell, ako je to znázornené v týchto bežných príkladoch:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
