---
title: 2419-nedá-na-enable-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065701"
---
# <a name="unable-to-enable-unified-auditing"></a>Nepodarilo sa zapnúť jednotného auditu

Pri pokuse povoliť jednotný auditovanie pre organizáciu balíka Office 365, môže zobraziť chyby podobné nasledovné:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Ak chcete vyriešiť tento problém, postupujte nasledovne:

1. [Pripojiť na Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Spustite nasledujúci cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkajte 60 minút pre predchádzajúce nastavenia prejavili.

4. Spustite nasledujúci príkaz v Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ďalšie informácie nájdete v nasledujúcich článkoch:

- [Pripojiť na Exchange Online PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Vypnutie Office 365 vyhľadávanie denník auditu](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
