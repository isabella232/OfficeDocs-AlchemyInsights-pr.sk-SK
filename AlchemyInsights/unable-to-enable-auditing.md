---
title: 2419-schopný-umožniť-umožniť-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510443"
---
# <a name="unable-to-enable-unified-auditing"></a>Nie je možné povoliť zjednotené auditovanie

Pri pokuse o povolenie zjednoteného auditovania pre vašu organizáciu sa môže zobraziť chyba podobná nasledovnej:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Ak chcete vyriešiť tento problém, postupujte nasledovne:

1. [Pripojte sa k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Spustite nasledujúci cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkajte 60 minút, kým sa predchádzajúce nastavenie prejaví.

4. Spustite nasledujúci príkaz v prostredí Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ďalšie informácie nájdete v nasledujúcich článkoch:

- [Pripojenie k prostrediu Exchange Online PowerShell pomocou viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Zapnutie alebo vypnutie vyhľadávania denníka auditu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
