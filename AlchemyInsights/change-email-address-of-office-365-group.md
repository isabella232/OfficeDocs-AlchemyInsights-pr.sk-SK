---
title: Zmena e-mailovej adresy Microsoft 365 skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930744"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Zmena e-mailovej adresy Microsoft 365 skupiny

E-mailovú adresu skupiny Microsoft 365 môžete zmeniť pomocou Centra spravovania. Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.

Ak chcete zmeniť primárnu SMTP adresu Microsoft 365, môžete použiť aj nasledujúci príkaz prostredia PowerShell Microsoft 365 EXO:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Príklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
