---
title: Povolenie DKIM pre konkrétnu doménu pomocou prostredia Exchange Online PowerShell
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525243"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Povolenie DKIM pre konkrétnu doménu pomocou prostredia Exchange Online PowerShell

Ak v centre spravovania nie je možné vytvoriť DNS záznamy DKIM, skúste použiť prostredie Exchange Online PowerShell. 

Ak chcete vytvoriť DNS záznam DKIM pomocou prostredia Exchange Online PowerShell, vykonajte tieto kroky:

1. Otvorte prostredie Windows PowerShell ako správca a spustite v opísanej postupnosti nasledovné príkazy:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ak máte problémy s pripojením k službe Exchange Online PowerShell, pozrite si tému [pripojenie k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Po pripojení k službe Exchange Online PowerShell spustite nasledujúci príkaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po úspešnom spustení príkazu vyššie spustite nasledujúci príkaz na ukončenie relácie prostredia Exchange Online PowerShell:

    `Remove-PSSession $Session` 



