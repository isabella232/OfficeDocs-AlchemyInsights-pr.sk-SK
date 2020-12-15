---
title: Používanie služby Microsoft Intune na spravovanie webového prístupu v prehliadači Microsoft Edge pre iOS a Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679607"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="62376-102">Používanie služby Microsoft Intune na spravovanie webového prístupu v prehliadači Microsoft Edge pre iOS a Android</span><span class="sxs-lookup"><span data-stu-id="62376-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="62376-103">Microsoft Edge pre iOS a Android umožňuje používateľovi prehľadávať web z viacerých, úplne oddelených profilov.</span><span class="sxs-lookup"><span data-stu-id="62376-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="62376-104">Najširšie možnosti ochrany údajov v službe Microsoft 365 sú k dispozícii, keď sa prihlásite na odber balíka Enterprise mobility + Security Suite, ktorý zahŕňa služby Microsoft Intune a Azure Active Directory Premium, ako napríklad podmienený prístup.</span><span class="sxs-lookup"><span data-stu-id="62376-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="62376-105">Na minimum budete chcieť nasadiť politiku podmieneného prístupu, ktorú (1) umožňuje používateľom pripojiť sa z mobilných zariadení na Microsoft Edge pre iOS a Android a že (2) implementuje politiku ochrany aplikácie Microsoft Intune, ktorá poskytuje zabezpečený zážitok z prehľadávania.</span><span class="sxs-lookup"><span data-stu-id="62376-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="62376-106">Ak chcete zistiť, ako môžete používať podmienený prístup a politiky, pozrite si tému:</span><span class="sxs-lookup"><span data-stu-id="62376-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="62376-107">Použitie politiky podmieneného prístupu služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="62376-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="62376-108">Vytvorenie politík ochrany aplikácií v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62376-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="62376-109">Používanie jediného prihlásenia pre službu Azure Active Directory – pripojené webové aplikácie v prehliadačoch chránených politikou</span><span class="sxs-lookup"><span data-stu-id="62376-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="62376-110">Použitie konfigurácie aplikácie na spravovanie prehľadávania</span><span class="sxs-lookup"><span data-stu-id="62376-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="62376-111">Povolenie používania len pracovných a školských kont</span><span class="sxs-lookup"><span data-stu-id="62376-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="62376-112">Nasadenie všeobecných politík konfigurácie aplikácií</span><span class="sxs-lookup"><span data-stu-id="62376-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="62376-113">Nasadenie politík konfigurácie aplikácií na ochranu údajov</span><span class="sxs-lookup"><span data-stu-id="62376-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="62376-114">Použitie aplikácie Microsoft Endpoint Manager na nasadenie politík konfigurácie aplikácií</span><span class="sxs-lookup"><span data-stu-id="62376-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="62376-115">Ďalšie informácie o prístupe k spravovaným denníkom aplikácií nájdete v téme [Používanie prehliadača Microsoft Edge pre iOS a Android na prístup k spravovaným denníkom aplikácií](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="62376-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
