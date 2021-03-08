---
title: Nastavenie ClientAccessServerEnabled na hodnotu True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525962"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastavenie ClientAccessServerEnabled na hodnotu True

Ak nie je možné otvoriť zašifrovanú e-mailovú správu a namiesto toho Zobraziť **rpmsg** prílohu, vykonajte tieto kroky:

1. Pripojte sa k službe Exchange Online PowerShell.

> [!NOTE]
> Ak sa chcete pripojiť k službe Exchange Online PowerShell, musíte sa prihlásiť pomocou globálneho správcu alebo konta správcu služby Exchange.

   a. Otvorte prostredie Windows PowerShell a spustite nasledujúci príkaz: `$UserCredential = Get-Credential`
b. V dialógovom okne **žiadosť o poverenia prostredia Windows PowerShell** zadajte svoje pracovné alebo školské konto a heslo, c. Kliknite na tlačidlo **OK**. 

2. Ak chcete vytvoriť novú reláciu, spustite nasledujúci príkaz:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spustite nasledujúci príkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Príkaz Spustiť.

4. Skontrolujte nastavenie **ClientAccessServerEnabled** . 

    a. Ak je nastavenie **ClientAccessServerEnabled** nastavená na **hodnotu False**, spustite nasledujúcu rutinu typu cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Vždy ukončite reláciu prostredia PowerShell pomocou nasledujúceho príkazu: `Remove-PSSession $Session`

Ďalšie informácie nájdete v téme [prostredie Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

