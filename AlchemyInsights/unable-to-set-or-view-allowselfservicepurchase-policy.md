---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158576"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="1e939-102">Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="1e939-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="1e939-103">Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase, zobrazí nasledujúce chybové hlásenie:</span><span class="sxs-lookup"><span data-stu-id="1e939-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="1e939-104">*HandleError: Nepodarilo sa načítať politiku produktu s PolicyId "AllowSelfServicePurchase", ErrorMessage-základné pripojenie bolo zatvorené: Vyskytla sa neočakávaná chyba pri odosielaní.*</span><span class="sxs-lookup"><span data-stu-id="1e939-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="1e939-105">Môže to byť spôsobené staršou verziou zabezpečenia transportnej vrstvy (TLS).</span><span class="sxs-lookup"><span data-stu-id="1e939-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="1e939-106">Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1,2 alebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="1e939-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="1e939-107">Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na 1,2, overenie a opakovanie.</span><span class="sxs-lookup"><span data-stu-id="1e939-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="1e939-108">V príkazovom riadku prostredia PowerShell (PS C:\) zadajte nasledovný príkaz na nastavenie protokolu TLS na verziu 1,2:</span><span class="sxs-lookup"><span data-stu-id="1e939-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="1e939-109">Overte, či protokol (y) TLS používa, s nasledujúcim príkazom:</span><span class="sxs-lookup"><span data-stu-id="1e939-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="1e939-110">Podľa potreby zopakujte príkazy získať alebo aktualizovať.</span><span class="sxs-lookup"><span data-stu-id="1e939-110">Retry the Get or Update commands as needed.</span></span>

