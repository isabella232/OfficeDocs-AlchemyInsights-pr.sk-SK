---
title: Zmena e-mailovej adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283260"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Zmena e-mailovej adresy skupiny Microsoft 365

Môžete zmeniť e-mailovú adresu skupiny Microsoft 365 pomocou admin Center. Stačí vybrať skupinu a vybrať @edit e-mailovú adresu.

Môžete použiť aj po príkaze EXO PowerShell zmeniť primárnu adresu SMTP skupiny Microsoft 365:

Súbor UnifiedGroup <Group Name> -primarysmtpaddress<new SMTP Address>

Príklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
