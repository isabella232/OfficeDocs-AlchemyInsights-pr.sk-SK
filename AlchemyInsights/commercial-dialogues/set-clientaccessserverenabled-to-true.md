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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994880"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastaviť ClientAccessServerEnabled na hodnotu True

Ak nemôžete otvoriť zašifrovanú e-mailovú správu a namiesto toho zobraziť prílohu **srpmsg,** vykonajte tieto kroky:

1. Pripojenie to Exchange Online PowerShell.

> [!NOTE]
> Ak sa chcete Exchange Online do prostredia PowerShell, musíte sa prihlásiť pomocou konta globálneho správcu Exchange správcu.

   a. Otvorte Windows PowerShell a potom spustite tento príkaz:`$UserCredential = Get-Credential`
b. V **dialógovom Windows PowerShell žiadosť o poverenia** zadajte svoje pracovné alebo školské konto a heslo c. Kliknite na tlačidlo **OK**. 

2. Vytvorte novú reláciu spustením tohto príkazu:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spustite nasledujúci príkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Spustenie `Get-IRMConfiguration` príkazu.

4. Skontrolujte **nastavenie ClientAccessServerEnabled.** 

    a. Ak **je hodnota ClientAccessServerEnabled** nastavená na hodnotu **False,** spustite nasledujúcu rutinu cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Reláciu prostredia PowerShell vždy zatvorte pomocou tohto príkazu: `Remove-PSSession $Session`

Ďalšie informácie nájdete v téme [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

