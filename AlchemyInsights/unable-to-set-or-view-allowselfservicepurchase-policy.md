---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826106"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="fd367-102">Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="fd367-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="fd367-103">Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase sa zobrazí toto chybové hlásenie:</span><span class="sxs-lookup"><span data-stu-id="fd367-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="fd367-104">*HandleError: Nepodarilo sa načítať politiku produktu s nastavením PolicyId 'AllowSelfServicePurchase', ErrorMessage – základné pripojenie sa uzavrelo: Pri odosielaní sa vyskytla neočakávaná chyba.*</span><span class="sxs-lookup"><span data-stu-id="fd367-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="fd367-105">Môže to byť spôsobené staršou verziou protokolu TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="fd367-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="fd367-106">Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1.2 alebo vyššiu.</span><span class="sxs-lookup"><span data-stu-id="fd367-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="fd367-107">Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na možnosť 1.2, overenie a zopakovanie pokusu.</span><span class="sxs-lookup"><span data-stu-id="fd367-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="fd367-108">Do príkazového riadka prostredia PowerShell (PS C: zadajte nasledujúci príkaz na nastavenie protokolu \) TLS na verziu 1.2):</span><span class="sxs-lookup"><span data-stu-id="fd367-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="fd367-109">Pomocou nasledujúceho príkazu overte protokol TLS, ktorý sa používa:</span><span class="sxs-lookup"><span data-stu-id="fd367-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="fd367-110">Podľa potreby znova skúste príkazy Získať alebo Aktualizovať.</span><span class="sxs-lookup"><span data-stu-id="fd367-110">Retry the Get or Update commands as needed.</span></span>

