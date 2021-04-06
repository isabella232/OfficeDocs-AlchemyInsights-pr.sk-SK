---
title: Obnovenie odstránenej skupiny Microsoft 365
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597458"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovenie odstránenej skupiny Microsoft 365

Odstránenú skupinu v Microsoft 365 alebo aplikáciu Microsoft Teams môžete obnoviť do 30 dní od odstránenia.

1. Prejdite do Centra [spravovania služby Microsoft 365 a](https://aka.ms/RestoreDeletedGroup) prihláste sa do zoznamu odstránených skupín a tímov.

    **Poznámka:** Prihláste sa pomocou konta, ktoré je priradené správcovi nájomníkovi alebo k role správcu skupín.

1. Vyberte odstránenú skupinu alebo aplikáciu Microsoft 365/Teams, ktorá sa má obnoviť, a kliknite na **položku Obnoviť skupinu**.

    Ak skupinu nemožno obnoviť z dôvodu konfliktnej adresy SMTP, pomocou nasledujúceho príkazu vyhľadajte objekt, ktorý je príčinou konfliktu, a odstráňte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V niektorých prípadoch môže trvať až 24 hodín, kým sa skupina a všetky jej údaje obnovia.

    Ďalšie informácie alebo informácie o obnovení skupín pomocou prostredia PowerShell nájdete v téme Obnovenie [odstránenej skupiny v službe Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)