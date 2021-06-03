---
title: Endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731867"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="a142f-102">Endpoint DLP not deployed to user's device</span><span class="sxs-lookup"><span data-stu-id="a142f-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="a142f-103">Ak sa nastavenie Ochrany pred stratou údajov (DLP) koncového bodu ešte v zariadení používateľa použilo, potvrďte, že spĺňate tieto požiadavky:</span><span class="sxs-lookup"><span data-stu-id="a142f-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="a142f-104">Windows 10 je v zariadení nainštalovaná zostava x64 1809 alebo novšia.</span><span class="sxs-lookup"><span data-stu-id="a142f-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="a142f-105">Je nainštalovaný anti malware client verzie 4.18.2009.7 alebo novšej.</span><span class="sxs-lookup"><span data-stu-id="a142f-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="a142f-106">Zariadenie je **jedným z** týchto zariadení:</span><span class="sxs-lookup"><span data-stu-id="a142f-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="a142f-107">Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="a142f-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="a142f-108">Hybridný Azure AD pripojený</span><span class="sxs-lookup"><span data-stu-id="a142f-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="a142f-109">Zaregistrované AAD</span><span class="sxs-lookup"><span data-stu-id="a142f-109">AAD registered</span></span>

- <span data-ttu-id="a142f-110">Ak chcete uplatniť akcie politiky, uistite sa, Chromium máte v koncovom zariadení nainštalovaný prehliadač Microsoft Chromium Edge.</span><span class="sxs-lookup"><span data-stu-id="a142f-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="a142f-111">Ďalšie požiadavky na nasadenie politiky DLP koncového bodu nájdete v téme Začíname s [ochrane pred stratou údajov koncových bodov.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="a142f-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>