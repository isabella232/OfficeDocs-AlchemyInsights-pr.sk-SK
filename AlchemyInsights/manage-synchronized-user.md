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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nedá sa nastaviť primárnu e-mailovú adresu alebo zmeniť používateľské atribúty

Ak Synchronizácia adresárov je povolené pre vaše prostredie, niektoré atribúty používateľa alebo objektu nie je možné zmeniť pomocou Microsoft 365 admin center.

Plne Spravovať synchronizáciu používateľov a všetky ich atribúty, použitie lokálnej služby active directory používatelia a skupiny riadenia konzoly (adsiedit.msc).  

Prípadne môžete jednotlivým používateľom alebo atribúty pre synchronizáciu používateľov pomocou powershell, ako je uvedené v týchto bežných príkladoch: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test používateľa" - priezvisko "User"-názov "Manager"-oddelenie "HR"
- Odstránenie MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com