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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074689"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vyradenie starších nástrojov vyhľadávania eDiscovery

V dôsledku novej a vylepšenej funkcie eDiscovery v centre dodržiavania súladu pre Microsoft 365 sa v nadchádzajúcich mesiacoch tieto staršie nástroje a commandlety služby eDiscovery prepustia:

- [Miestne blokovanie eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a miestne [blokovanie blokovania](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v Exchange spravovania.

- Rutiny Exchange Online PowerShell, ktoré podporujú In-Place eDiscovery a blokovania In-Place blokovania. (Tieto rutiny typu cmdlet sa spolu identifikujú ako rutiny typu cmdlet *-MailboxSearch.) Patria sem nasledujúce rutiny cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutina typu cmdlet [search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v Exchange Online PowerShell.
- Nasledujúce operácie v rozhraní Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová os na vyradenie:**
- **1. júla 2020** Už nemôžete vytvárať nové vyhľadávania a zadržanie, ale môžete spustiť, upraviť a odstrániť existujúce vyhľadávania na vlastné riziko. Podpora spoločnosti Microsoft už nepodporuje In-Place eDiscovery & blokovania blokovania uchová v EAC.
    
- Funkcie In-Place eDiscovery & Holds v EAC z **1. októbra 2020** sa umiestnia do režimu iba na čítanie, takže môžete odstrániť iba existujúce vyhľadávania a blokovania.

**Ďalšie informácie nájdete v téme:**

 - [Migrácia starších vyhľadávaní eDiscovery a blokovania ich Centrum dodržiavania súladu pre Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vyradenie starších nástrojov vyhľadávania eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčastejšie otázky o In-Place eDiscovery a In-Place blokovania elektronického vyhľadávania](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



