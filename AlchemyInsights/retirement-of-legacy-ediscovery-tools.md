---
title: Vyradenie starších nástrojov vyhľadávania eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798564"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vyradenie starších nástrojov vyhľadávania eDiscovery

V dôsledku novej a vylepšenej funkcie eDiscovery v centre dodržiavania súladu pre Microsoft 365 sa v nadchádzajúcich mesiacoch tieto staršie nástroje a commandlety služby eDiscovery prepustia:

- [Miestne blokovanie eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [a miestne blokovanie blokovania](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v Centre spravovania pre Exchange.

- Rutiny typu cmdlet prostredia PowerShell služby Exchange Online, ktoré In-Place eDiscovery a blokovania In-Place blokovania údajov. (Tieto rutiny typu cmdlet sa spolu identifikujú ako rutiny typu cmdlet *-MailboxSearch.) Patria sem nasledujúce rutiny cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutina typu cmdlet [search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.
- Nasledujúce operácie v rozhraní API webových služieb Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová os na vyradenie:**
- **1. júla 2020** Už nemôžete vytvárať nové vyhľadávania a zadržanie, ale môžete spustiť, upraviť a odstrániť existujúce vyhľadávania na vlastné riziko. Podpora spoločnosti Microsoft už nepodporuje In-Place eDiscovery & blokovania blokovania uchová v EAC.
    
- Funkcie In-Place eDiscovery & Holds v EAC z **1. októbra 2020** sa umiestnia do režimu iba na čítanie, takže môžete odstrániť iba existujúce vyhľadávania a blokovania.

**Ďalšie informácie nájdete v téme:**

 - [Migrácia starších vyhľadávaní eDiscovery a blokovania ich zadržania do Centra dodržiavania súladu pre Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vyradenie starších nástrojov vyhľadávania eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčastejšie otázky o In-Place eDiscovery a In-Place blokovania elektronického vyhľadávania](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



