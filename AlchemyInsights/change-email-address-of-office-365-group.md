---
title: Zmena e-mailovej adresy skupiny Microsoft 365
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819059"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Zmena e-mailovej adresy skupiny Microsoft 365

E-mailovú adresu skupiny v Microsoft 365 môžete zmeniť pomocou Centra spravovania. Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.

Ak chcete zmeniť primárnu SMTP adresu skupiny Microsoft 365, môžete použiť aj tento príkaz prostredia PowerShell EXO:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Príklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
