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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="a6fae-102">Nie je možné povoliť zjednotené auditovanie</span><span class="sxs-lookup"><span data-stu-id="a6fae-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="a6fae-103">Pri pokuse o povolenie zjednoteného auditovania pre vašu organizáciu sa môže zobraziť chybové hlásenie podobné nasledujúcemu:</span><span class="sxs-lookup"><span data-stu-id="a6fae-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="a6fae-104">Ak chcete tento problém vyriešiť, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="a6fae-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="a6fae-105">[Pripojte sa k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="a6fae-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="a6fae-106">Spustite nasledujúcu rutinu typu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a6fae-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="a6fae-107">Počkajte na 60 minút, kým sa predchádzajúce nastavenie prejaví.</span><span class="sxs-lookup"><span data-stu-id="a6fae-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="a6fae-108">Spustite nasledujúci príkaz v prostredí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a6fae-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="a6fae-109">Ďalšie informácie nájdete v nasledujúcich článkoch:</span><span class="sxs-lookup"><span data-stu-id="a6fae-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="a6fae-110">Pripojenie k službe Exchange Online PowerShell pomocou viacnásobného overovania</span><span class="sxs-lookup"><span data-stu-id="a6fae-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="a6fae-111">Zapnutie alebo vypnutie vyhľadávania denníka auditu</span><span class="sxs-lookup"><span data-stu-id="a6fae-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
