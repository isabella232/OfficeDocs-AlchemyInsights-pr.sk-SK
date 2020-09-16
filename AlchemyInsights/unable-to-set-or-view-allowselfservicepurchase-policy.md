---
title: Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735214"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="46aa3-102">Nie je možné nastaviť alebo zobraziť politiku AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="46aa3-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="46aa3-103">Pri pokuse o nastavenie alebo zobrazenie politiky AllowSelfServicePurchase sa zobrazí nasledujúce chybové hlásenie:</span><span class="sxs-lookup"><span data-stu-id="46aa3-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="46aa3-104">*HandleError: Nepodarilo sa načítať politiku produktov s PolicyId ' AllowSelfServicePurchase ', ErrorMessage-základné pripojenie bolo ukončené: na odoslanie sa vyskytla neočakávaná chyba.*</span><span class="sxs-lookup"><span data-stu-id="46aa3-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="46aa3-105">Môže to byť spôsobené staršou verziou zabezpečenia Transport Layer (TLS).</span><span class="sxs-lookup"><span data-stu-id="46aa3-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="46aa3-106">Ak chcete pripojiť službu MSCommerce, musíte použiť TLS 1,2 alebo novšiu.</span><span class="sxs-lookup"><span data-stu-id="46aa3-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="46aa3-107">Vyskúšajte nasledujúce kroky na zapnutie alebo nastavenie protokolu TLS na 1,2, overenie a opakovanie.</span><span class="sxs-lookup"><span data-stu-id="46aa3-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="46aa3-108">V príkazovom riadku prostredia PowerShell (PS C: \) Ak chcete nastaviť protokol TLS na verziu 1,2, zadajte nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="46aa3-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="46aa3-109">Overte, či sa používajú protokoly TLS s týmto príkazom:</span><span class="sxs-lookup"><span data-stu-id="46aa3-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="46aa3-110">Podľa potreby zopakujte príkazy získať alebo aktualizovať.</span><span class="sxs-lookup"><span data-stu-id="46aa3-110">Retry the Get or Update commands as needed.</span></span>

