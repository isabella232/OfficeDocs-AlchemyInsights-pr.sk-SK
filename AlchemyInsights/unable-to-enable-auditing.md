---
title: 2419 – nedá sa povoliť – auditovanie
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767614"
---
# <a name="unable-to-enable-unified-auditing"></a>Nie je možné povoliť zjednotené auditovanie

Pri pokuse o povolenie zjednoteného auditovania pre vašu organizáciu sa môže zobraziť chybové hlásenie podobné nasledujúcemu:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Ak chcete tento problém vyriešiť, postupujte podľa týchto krokov:

1. [Pripojte sa k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Spustite nasledujúcu rutinu typu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkajte na 60 minút, kým sa predchádzajúce nastavenie prejaví.

4. Spustite nasledujúci príkaz v prostredí Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ďalšie informácie nájdete v nasledujúcich článkoch:

- [Pripojenie k službe Exchange Online PowerShell pomocou viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Zapnutie alebo vypnutie vyhľadávania denníka auditu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
