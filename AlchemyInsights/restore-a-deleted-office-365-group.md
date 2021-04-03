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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505705"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovenie odstránenej skupiny Microsoft 365

Odstránenú skupinu v Microsoft 365 alebo aplikáciu Microsoft Teams môžete obnoviť do 30 dní od odstránenia.

1. Ak sa chcete prihlásiť do Centra spravovania služby Microsoft 365 a vytvoriť zoznam odstránených skupín a tímov, prejdite do Centra [spravovania služby Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Poznámka:** Prihláste sa pomocou konta, ktoré je priradené správcovi nájomníkovi alebo k role správcu skupín.

1. Vyberte odstránenú skupinu alebo aplikáciu Microsoft 365/Teams, ktorá sa má obnoviť, a kliknite na **položku Obnoviť skupinu**.

    Ak skupinu nemožno obnoviť z dôvodu konfliktnej adresy SMTP, pomocou nasledujúceho príkazu vyhľadajte objekt, ktorý je príčinou konfliktu, a odstráňte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V niektorých prípadoch môže trvať až 24 hodín, kým sa skupina a všetky jej údaje obnovia.

    Ďalšie informácie alebo informácie o obnovení skupín pomocou prostredia PowerShell nájdete v téme Obnovenie [odstránenej skupiny v službe Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)