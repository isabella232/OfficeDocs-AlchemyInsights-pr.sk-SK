---
title: Obnovenie odstránenej Microsoft 365 skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959041"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovenie odstránenej Microsoft 365 skupiny

Odstránenú skupinu alebo Microsoft 365 môžete obnoviť Microsoft Teams do 30 dní od odstránenia.

1. Prejdite na [Centrum spravovania služby Microsoft 365](https://aka.ms/RestoreDeletedGroup) a prihláste sa do zoznamu odstránených skupín a tímov.

    **Poznámka:** Prihláste sa pomocou konta, ktoré je priradené správcovi nájomníkovi alebo k role správcu skupín.

1. Vyberte odstránené skupiny Microsoft 365 alebo skupiny Teams ktoré sa majú obnoviť, a kliknite na **položku Obnoviť skupinu**.

    Ak skupinu nemožno obnoviť z dôvodu konfliktnej adresy SMTP, pomocou nasledujúceho príkazu vyhľadajte objekt, ktorý je príčinou konfliktu, a odstráňte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V niektorých prípadoch môže trvať až 24 hodín, kým sa skupina a všetky jej údaje obnovia.

    Ďalšie informácie alebo informácie o obnovení skupín pomocou prostredia PowerShell nájdete v téme Obnovenie [odstránenej Microsoft 365 skupiny.](https://go.microsoft.com/fwlink/?linkid=867802)