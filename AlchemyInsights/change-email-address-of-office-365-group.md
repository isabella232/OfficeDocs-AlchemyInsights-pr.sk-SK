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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580672"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Zmena e-mailovej adresy skupiny Microsoft 365

E-mailovú adresu skupiny Microsoft 365 môžete zmeniť pomocou Centra spravovania. Stačí vybrať skupinu a vybrať @edit e-mailovú adresu.

Môžete tiež použiť nasledujúci príkaz EXO PowerShell zmeniť primárnu adresu SMTP skupiny Microsoft 365:

Súbor UnifiedGroup <Group Name> - PrimarySmtpAddress<new SMTP Address>

Príklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
