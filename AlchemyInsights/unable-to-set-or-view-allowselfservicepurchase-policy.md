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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091762"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="da6fb-102">Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="da6fb-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="da6fb-103">Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase, zobrazí nasledujúce chybové hlásenie:</span><span class="sxs-lookup"><span data-stu-id="da6fb-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="da6fb-104">*HandleError: Nepodarilo sa načítať politiku produktu s PolicyId "AllowSelfServicePurchase", ErrorMessage-základné pripojenie bolo zatvorené: Vyskytla sa neočakávaná chyba pri odosielaní.*</span><span class="sxs-lookup"><span data-stu-id="da6fb-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="da6fb-105">Môže to byť spôsobené staršou verziou zabezpečenia transportnej vrstvy (TLS).</span><span class="sxs-lookup"><span data-stu-id="da6fb-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="da6fb-106">Ak chcete pripojiť službu MSCommerce, musíte použiť protokol TLS 1,2 alebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="da6fb-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="da6fb-107">Vyskúšajte nasledujúce kroky na zapnutie/nastavenie protokolu TLS na 1,2, overenie a opakovanie.</span><span class="sxs-lookup"><span data-stu-id="da6fb-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="da6fb-108">V príkazovom riadku prostredia PowerShell (PS C:\) zadajte nasledovný príkaz na nastavenie protokolu TLS na verziu 1,2:</span><span class="sxs-lookup"><span data-stu-id="da6fb-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="da6fb-109">\[NET. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="da6fb-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="da6fb-110">Overte, či protokol (y) TLS používa, s nasledujúcim príkazom:</span><span class="sxs-lookup"><span data-stu-id="da6fb-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="da6fb-111">\[NET. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="da6fb-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="da6fb-112">Podľa potreby zopakujte príkazy získať alebo aktualizovať.</span><span class="sxs-lookup"><span data-stu-id="da6fb-112">Retry the Get or Update commands as needed.</span></span>

