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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="ade63-102">Povolenie DKIM pre konkrétnu doménu pomocou prostredia Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="ade63-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="ade63-103">Ak v centre spravovania nie je možné vytvoriť DNS záznamy DKIM, skúste použiť prostredie Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ade63-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="ade63-104">Ak chcete vytvoriť DNS záznam DKIM pomocou prostredia Exchange Online PowerShell, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="ade63-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="ade63-105">Otvorte prostredie Windows PowerShell ako správca a spustite v opísanej postupnosti nasledovné príkazy:</span><span class="sxs-lookup"><span data-stu-id="ade63-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="ade63-106">a.</span><span class="sxs-lookup"><span data-stu-id="ade63-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="ade63-107">b.</span><span class="sxs-lookup"><span data-stu-id="ade63-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="ade63-108">c.</span><span class="sxs-lookup"><span data-stu-id="ade63-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="ade63-109">Ak máte problémy s pripojením k službe Exchange Online PowerShell, pozrite si tému [pripojenie k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="ade63-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="ade63-110">Po pripojení k službe Exchange Online PowerShell spustite nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="ade63-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="ade63-111">Po úspešnom spustení príkazu vyššie spustite nasledujúci príkaz na ukončenie relácie prostredia Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ade63-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



