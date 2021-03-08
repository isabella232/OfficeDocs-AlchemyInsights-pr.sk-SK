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
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="5e4ef-102">Nastavenie ClientAccessServerEnabled na hodnotu True</span><span class="sxs-lookup"><span data-stu-id="5e4ef-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="5e4ef-103">Ak nie je možné otvoriť zašifrovanú e-mailovú správu a namiesto toho Zobraziť **rpmsg** prílohu, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="5e4ef-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="5e4ef-104">Pripojte sa k službe Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="5e4ef-105">Ak sa chcete pripojiť k službe Exchange Online PowerShell, musíte sa prihlásiť pomocou globálneho správcu alebo konta správcu služby Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="5e4ef-106">a.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-106">a.</span></span> <span data-ttu-id="5e4ef-107">Otvorte prostredie Windows PowerShell a spustite nasledujúci príkaz: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="5e4ef-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="5e4ef-108">b.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-108">b.</span></span> <span data-ttu-id="5e4ef-109">V dialógovom okne **žiadosť o poverenia prostredia Windows PowerShell** zadajte svoje pracovné alebo školské konto a heslo, c.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="5e4ef-110">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-110">Click **OK**.</span></span> 

2. <span data-ttu-id="5e4ef-111">Ak chcete vytvoriť novú reláciu, spustite nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="5e4ef-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="5e4ef-112">a.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-112">a.</span></span> <span data-ttu-id="5e4ef-113">Spustite nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="5e4ef-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="5e4ef-114">`Get-IRMConfiguration`Príkaz Spustiť.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="5e4ef-115">Skontrolujte nastavenie **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="5e4ef-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="5e4ef-116">a.</span><span class="sxs-lookup"><span data-stu-id="5e4ef-116">a.</span></span> <span data-ttu-id="5e4ef-117">Ak je nastavenie **ClientAccessServerEnabled** nastavená na **hodnotu False**, spustite nasledujúcu rutinu typu cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="5e4ef-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="5e4ef-118">Vždy ukončite reláciu prostredia PowerShell pomocou nasledujúceho príkazu: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="5e4ef-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="5e4ef-119">Ďalšie informácie nájdete v téme [prostredie Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="5e4ef-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

