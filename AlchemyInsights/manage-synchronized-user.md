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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380520"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nedá sa nastaviť primárnu e-mailovú adresu alebo zmeniť používateľské atribúty

Ak je povolená Synchronizácia adresárov pre vaše prostredie niektoré atribúty používateľa alebo objektu nie je možné zmeniť pomocou Admin Center.
Plne Spravovať synchronizáciu používateľov a všetky ich atribúty, použitie lokálnej služby active directory používatelia a skupiny riadenia konzoly (adsiedit.msc).  

Prípadne môžete jednotlivým používateľom alebo atribúty pre synchronizáciu používateľov pomocou powershell, ako je uvedené v týchto bežných príkladoch: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test používateľa" - priezvisko "User"-názov "Manager"-oddelenie "HR"
- Odstránenie MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com