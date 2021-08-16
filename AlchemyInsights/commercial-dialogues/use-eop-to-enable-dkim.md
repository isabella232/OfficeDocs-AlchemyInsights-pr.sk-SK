---
title: Použitie Exchange Online PowerShell na povolenie DKIM pre konkrétnu doménu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070330"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Použitie Exchange Online PowerShell na povolenie DKIM pre konkrétnu doménu

Ak nemôžete vytvoriť DNS záznamy DKIM v centre spravovania, skúste použiť Exchange Online PowerShell. 

Ak chcete vytvoriť DNS záznam DKIM pomocou Exchange Online PowerShell, vykonajte tieto kroky:

1. Otvorte Windows PowerShell ako správca a spustite nasledujúce príkazy v popísanej postupnosti:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ak máte problémy s pripojením k Exchange Online PowerShell, pozrite si [Pripojenie na Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Po pripojení k Exchange Online PowerShell spustite tento príkaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po úspešnom spustení príkazu uvedeného vyššie spustite nasledujúci príkaz, ktorý ukončí Exchange Online relácie prostredia PowerShell:

    `Remove-PSSession $Session` 



