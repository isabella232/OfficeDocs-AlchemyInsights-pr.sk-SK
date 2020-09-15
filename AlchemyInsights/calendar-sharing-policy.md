---
title: Politika zdieľania kalendára 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684245"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Chyba politiky pri zdieľaní kalendára

1. Vykonajte niektorý z týchto krokov, ktoré zodpovedajú vašej situácii:
    - Pripojte sa k službe Exchange Online pomocou vzdialeného prostredia PowerShell. Ďalšie informácie nájdete v téme [pripojenie k službe Exchange Online pomocou vzdialeného prostredia PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokálnom serveri Otvorte prostredie Exchange Management Shell.
2. Určenie politiky zdieľania, ktorá je priradená používateľovi. Ak to chcete urobiť, spustite nasledujúci príkaz a zaznamenajte si politiku, ktorá sa vrátila:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualizujte politiku zdieľania pre používateľa. Postupujte takto:
    - Otvorte Centrum spravovania pre Exchange.
    - Kliknite na položku **organizácia**a potom dvakrát kliknite na politiku, ktorá je priradená používateľovi v rámci **individuálneho zdieľania**. Toto je politika, ktorá bola vrátená v kroku 2.
    - Na stránke pravidlo zdieľania vyberte úroveň zdieľania kalendára, ktorú chcete povoliť v časti **určenie informácií, ktoré chcete zdieľať**. kliknite na tlačidlo **Uložiť**.

Ďalšie informácie nájdete v téme: [politika nepovoľuje udeliť povolenia na úrovni jednej alebo viacerým príjemcom pri pokuse o zdieľanie kalendára](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
