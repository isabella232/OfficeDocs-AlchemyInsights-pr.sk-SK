---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007805"
---
# <a name="unable-to-enable-unified-auditing"></a>Zjednotené auditovanie sa nedá povoliť

Pri pokuse o povolenie jednotného auditovania pre vašu organizáciu sa môže zobraziť chyba podobná tejto:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Ak chcete tento problém vyriešiť, postupujte takto:

1. [Pripojenie to Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Spustite nasledujúcu rutinu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkajte 60 minút, kým sa prejaví predchádzajúce nastavenie.

4. V prostredí PowerShell Exchange Online nasledujúci príkaz:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ďalšie informácie nájdete v nasledujúcich článkoch:

- [Pripojenie do Exchange Online PowerShell pomocou viacfaktorového overovania](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Zapnutie alebo vypnutie vyhľadávania denníka auditu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
