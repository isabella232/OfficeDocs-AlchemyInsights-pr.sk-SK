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
# <a name="unable-to-change-username"></a>Nie je možné zmeniť meno používateľa

V niektorých prípadoch, UPN (UserPrincipalName) zmeny nie sú šírené do cloudu. Chyby overenia sa môžu zobraziť na portáli služieb Office 365 alebo sa môžu zmeniť meno používateľa alebo e-mailovú adresu. Ak chcete vyriešiť tento problém, manuálne nastaviť UserPrincipalName pomocou tohto príkazu prostredia PowerShell.

**Príklad: Premenovanie používateľa**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Tento príkaz premenuje davidc@contoso.com na davidchew@contoso.com.

Ďalšie informácie nájdete v téme [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).