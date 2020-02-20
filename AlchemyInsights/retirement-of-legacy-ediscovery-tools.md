---
title: Odchod do dôchodku Legacy eDiscovery nástroje
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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157708"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Odchod do dôchodku Legacy eDiscovery nástroje

V dôsledku nových a vylepšených funkcií eDiscovery v Microsoft 365 Compliance Center, nasledujúce staršie eDiscovery nástroje a commandlets bude dôchodku v najbližších mesiacoch:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [in-miesto drží](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v Exchange Admin Center.

- Rutiny cmdlet prostredia Exchange Online PowerShell, ktoré podporujú in-Place eDiscovery a na mieste drží. (Tieto rutiny cmdlet sú súhrnne identifikované ako *-MailboxSearch rutiny cmdlet.) To zahŕňa nasledujúce rutiny cmdlet:

    - [Nové-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutiny cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.
- Nasledujúce operácie v rozhraní API webových služieb Exchange:
    - [Getsearchablepoštové schránky](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonpoštové schránky](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonpoštové schránky](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová os pre odchod do dôchodku**:
- 1. apríla, 2020: nebudete môcť vytvárať nové vyhľadávania a zadržania, ale stále môžete spúšťať, upravovať a odstraňovať existujúce vyhľadávania na vlastné riziko. Microsoft Support už nebude podporovať in-Place eDiscovery & drží v EAC.

- 1. júl 2020: in-Place eDiscovery & drží funkčnosť v EAC budú umiestnené v Read-Only režime. To znamená, že budete môcť odstrániť len existujúce vyhľadávania a ich podržaní.

**Ďalšie informácie nájdete v téme**:

 - [Migrovať staršie eDiscovery vyhľadávania a drží na Microsoft 365 Compliance Center](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Odchod do dôchodku Legacy eDiscovery nástroje](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčastejšie otázky o in-Place eDiscovery a in-Place drží](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



