---
title: 618 politika zdieľania kalendára
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373014"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Chyba politiky pri zdieľaní kalendára

1. Vykonajte jeden z nasledujúcich, ako je vhodné pre vašu situáciu:
    - Pripojenie k službe Exchange Online pomocou vzdialeného PowerShell. Ďalšie informácie nájdete v téme [pripojenie k službe Exchange Online pomocou vzdialeného PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokálnom serveri, Otvorte prostredie Exchange Management Shell.
2. Určenie politiky zdieľania priradenej používateľovi. Vykonáte to spustením nasledujúceho príkazu a poznačte si politiku vrátil:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualizujte politiku zdieľania pre používateľa. Postupujte takto:
    - Otvorte Exchange Admin Center.
    - Kliknite na položku **organizácia**a potom dvakrát kliknite na politiku priradenú používateľovi v časti **individuálne zdieľanie**. Toto je politika, ktorá bola vrátená v kroku 2.
    - Na stránke pravidlo zdieľania vyberte úroveň zdieľania kalendára, ktorú chcete povoliť v časti **určenie informácií, ktoré chcete zdieľať**; kliknite na tlačidlo **Uložiť**.

Ďalšie informácie nájdete: ["politika neumožňuje udelenie povolenia na tejto úrovni jeden alebo viac príjemcov" chyba, keď používateľ pokúsi zdieľať kalendár](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
