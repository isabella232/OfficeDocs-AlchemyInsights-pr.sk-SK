---
title: Použitie služby Microsoft Intune na spravovanie prístupu na web v aplikácii Microsoft Edge pre iOS a Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989714"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="10abc-102">Použitie služby Microsoft Intune na spravovanie prístupu na web v aplikácii Microsoft Edge pre iOS a Android</span><span class="sxs-lookup"><span data-stu-id="10abc-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="10abc-103">Microsoft Edge pre iOS a Android umožňuje používateľovi prehľadávať web z viacerých úplne samostatných profilov.</span><span class="sxs-lookup"><span data-stu-id="10abc-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="10abc-104">Keď sa prihlásite na odber balíka Enterprise Mobility + Security, ktorý zahŕňa funkcie Microsoft Intune a Azure Active Directory Premium, napríklad podmienený prístup, k dispozícii sú možnosti širokej ochrany údajov služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="10abc-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="10abc-105">Budete chcieť nasadiť minimálne politiku podmieneného prístupu, ktorá (1) umožní používateľom pripojiť sa z mobilných zariadení k Microsoft Edgeu pre iOS a Android a (2) implementuje politiku ochrany aplikácie Microsoft Intune, ktorá poskytuje chránený zážitok z prehľadávania.</span><span class="sxs-lookup"><span data-stu-id="10abc-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="10abc-106">Ak chcete porozumieť tomu, ako môžete používať podmienený prístup a politiky, pozrite si téme:</span><span class="sxs-lookup"><span data-stu-id="10abc-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="10abc-107">Použitie politík podmieneného prístupu v službe Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="10abc-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="10abc-108">Vytvorenie politík ochrany aplikácií od Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="10abc-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="10abc-109">Používanie jediného prihlásenia pre webové aplikácie pripojené k službe Azure Active Directory v prehliadačoch chránených politikami</span><span class="sxs-lookup"><span data-stu-id="10abc-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="10abc-110">Použitie konfigurácie aplikácie na spravovanie prehľadávania</span><span class="sxs-lookup"><span data-stu-id="10abc-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="10abc-111">Povoliť používanie iba pracovných a školských kont</span><span class="sxs-lookup"><span data-stu-id="10abc-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="10abc-112">Nasadenie všeobecných politík konfigurácie aplikácií</span><span class="sxs-lookup"><span data-stu-id="10abc-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="10abc-113">Nasadenie politík konfigurácie aplikácií na ochranu údajov</span><span class="sxs-lookup"><span data-stu-id="10abc-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="10abc-114">Na nasadenie politík konfigurácie aplikácií použite Microsoft Endpoint Manager</span><span class="sxs-lookup"><span data-stu-id="10abc-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="10abc-115">Informácie o prístupe k denníkom spravovaných aplikácií nájdete v téme Prístup k denníkom spravovaných aplikácií pomocou aplikácie [Microsoft Edge pre iOS a Android.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="10abc-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
