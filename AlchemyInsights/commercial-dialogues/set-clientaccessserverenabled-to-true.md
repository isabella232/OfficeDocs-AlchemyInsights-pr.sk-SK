---
title: Nastaviť ClientAccessServerEnabled na hodnotu True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320371"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastaviť ClientAccessServerEnabled na hodnotu True

Ak nemôžete otvoriť zašifrovanú e-mailovú správu a namiesto toho zobraziť prílohu **srpmsg,** vykonajte tieto kroky:

1. Pripojenie to Exchange Online PowerShell.

    **Poznámka:** Ak sa chcete pripojiť Exchange Online prostredí PowerShell, musíte sa prihlásiť pomocou konta globálneho správcu Exchange správcu.

   a. Otvorte Windows PowerShell a potom spustite tento príkaz:`$UserCredential = Get-Credential`
   b. V **dialógovom Windows PowerShell Žiadosť o poverenia** zadajte svoje pracovné alebo školské konto a heslo c. Kliknite na tlačidlo **OK**. 

2. Vytvorte novú reláciu spustením tohto príkazu:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spustite nasledujúci príkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Spustenie `Get-IRMConfiguration` príkazu.

4. Skontrolujte **nastavenie ClientAccessServerEnabled.** 

    a. Ak **je hodnota ClientAccessServerEnabled** nastavená na hodnotu **False,** spustite nasledujúcu rutinu cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tip:** Reláciu prostredia powershell vždy zatvorte pomocou tohto príkazu: `Remove-PSSession $Session`

Ďalšie informácie nájdete v téme [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

