---
title: 618 Politika zdieľania kalendára
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091618"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Chyba politiky pri zdieľaní kalendára

1. V prípade potreby vykonajte niektorý z týchto krokov:
    - Pripojenie sa Exchange Online pomocou prostredia Remote PowerShell. Ďalšie informácie nájdete v téme [Pripojenie a Exchange Online remote PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Na lokálnom serveri otvorte prostredie Exchange Management Shell.
2. Určte politiku zdieľania, ktorá je priradená používateľovi. Ak to chcete urobiť, spustite nasledujúci príkaz a všimnite si vrátenú politiku:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualizujte politiku zdieľania pre používateľa. Postupujte takto:
    - Otvorte Centrum Exchange spravovania.
    - Kliknite **na** položku Organizácia a potom dvakrát kliknite na politiku priradenú používateľovi v časti **Individuálne zdieľanie**. Toto je politika, ktorá sa vrátila v kroku 2.
    - Na stránke Pravidlo zdieľania vyberte v časti Zadajte informácie, ktoré chcete zdieľať, úroveň zdieľania kalendára, ktorú **chcete povoliť.** kliknite na **položku Uložiť.**

Ďalšie informácie nájdete v téme: Chyba "Politika neumožňuje udeliť povolenia na tejto úrovni najmenej niektorému príjemcovi" v prípade, že sa používateľ pokúša [zdieľať kalendár.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
