---
title: Odchod starších nástrojov elektronického vyhľadávania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902635"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Odchod starších nástrojov elektronického vyhľadávania

V dôsledku novej a vylepšenej funkcie elektronického vyhľadávania v centre dodržiavania súladu pre Microsoft 365 sa v nasledujúcich mesiacoch vyplatí nasledujúci starší nástroj eDiscovery a príkazové aplety:

- [Miestne elektronické vyhľadávanie](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [miestne priestory](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v centre spravovania pre Exchange.

- Rutiny cmdlet prostredia PowerShell služby Exchange Online, ktoré podporujú miestne elektronické vyhľadávanie a miestne zadržania. (Tieto rutiny typu cmdlet sa spoločne identifikujú ako rutiny cmdlet *-MailboxSearch.) Zahŕňa tieto rutiny typu cmdlet:

    - [Nové – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutina cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.
- Nasledujúce operácie v rozhraní API webových služieb Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Rozšírené elektronické vyhľadávanie v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová os na odchod do dôchodku**:
- **1. júl 2020** Už nie je možné vytvárať nové vyhľadávania a zadržania, ale môžete spustiť, upraviť a odstrániť existujúce vyhľadávania na vlastné riziko. Podpora spoločnosti Microsoft už nepodporuje miestne elektronické vyhľadávanie & v systéme EAC.
    
- **1. október 2020** Miestne elektronické vyhľadávanie & zachová funkčnosť v systéme EAC sa umiestni do režimu iba na čítanie, takže môžete odstrániť iba existujúce vyhľadávania a zadržania.

**Ďalšie informácie nájdete v témach**:

 - [Migrácia starších vyhľadávaní vyhľadávania eDiscovery a zadržania v centre zabezpečenia dodržiavania súladu pre Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Odchod starších nástrojov elektronického vyhľadávania](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčastejšie otázky týkajúce sa miestneho elektronického vyhľadávania a lokálnych zadržaní](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



