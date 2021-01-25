---
title: Problémy s vývojom aplikácií
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974768"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="8da07-102">Problémy s vývojom aplikácií</span><span class="sxs-lookup"><span data-stu-id="8da07-102">Issues developing applications</span></span>

<span data-ttu-id="8da07-103">Ak chcete riešiť najbežnejšie problémy pri budovaní aplikácií služby Azure Active Directory (AD), prečítajte si tieto články:</span><span class="sxs-lookup"><span data-stu-id="8da07-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="8da07-104">Zobrazujem problémy s prihlásením do aplikácie (s) iba pomocou prehliadača Chrome</span><span class="sxs-lookup"><span data-stu-id="8da07-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="8da07-105">Neviem, ako zmeniť predvolené nastavenia tokenu životnosti pre moju aplikáciu</span><span class="sxs-lookup"><span data-stu-id="8da07-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="8da07-106">Som zmätená o tom, ako funguje súhlas so žiadosťou</span><span class="sxs-lookup"><span data-stu-id="8da07-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="8da07-107">Neviem, ako udeliť povolenia mojej aplikácii</span><span class="sxs-lookup"><span data-stu-id="8da07-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="8da07-108">Nechápem rozdiel medzi delegovanými povoleniami a povoleniami na aplikácie</span><span class="sxs-lookup"><span data-stu-id="8da07-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="8da07-109">\***Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="8da07-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="8da07-110">Od 30. júna 2020, už nebudeme pridávať žiadne nové funkcie do služby Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="8da07-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="8da07-111">Budeme aj naďalej poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudú poskytovať aktualizácie funkcií.</span><span class="sxs-lookup"><span data-stu-id="8da07-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="8da07-112">Od 30. júna 2022, ukončíme podporu pre ADAL a AAD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="8da07-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="8da07-113">Výsledkom tejto podmienky sú tieto dôsledky:</span><span class="sxs-lookup"><span data-stu-id="8da07-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="8da07-114">Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však mať žiadne technické podpory ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="8da07-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="8da07-115">Aplikácie, ktoré používajú AAD Graph po uplynutí tohto času, už nemusia dostávať odpovede od koncového bodu grafu AAD</span><span class="sxs-lookup"><span data-stu-id="8da07-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="8da07-116">_ *Migrácia ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="8da07-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="8da07-117">Ak používate aplikácie spoločnosti Microsoft, odporúčame vám aktualizovať knižnicu Microsoft Authentication Library (MSAL), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="8da07-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="8da07-118">Toto odporúčanie je v kontexte Microsoftu, ktorým sa iniciuje proces prechodu svojich aplikácií na MSAL podľa termínu ukončenia podpory.</span><span class="sxs-lookup"><span data-stu-id="8da07-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="8da07-119">Migrácia aplikácií spoločnosti Microsoft na MSAL zabezpečuje, že aplikácie budú mať prospech z pokračujúcich funkcií zabezpečenia a vylepšení funkcie MSAL.</span><span class="sxs-lookup"><span data-stu-id="8da07-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8da07-120">Prečítajte si najčastejšie otázky o ADAL</span><span class="sxs-lookup"><span data-stu-id="8da07-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="8da07-121">Informácie o tom, ako migrovať aplikácie na základe jednotlivých platforiem</span><span class="sxs-lookup"><span data-stu-id="8da07-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="8da07-122">Ak potrebujete pomoc pri pochopení, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="8da07-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8da07-123">Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií, ktoré nie sú Microsoft ADAL v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="8da07-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8da07-124">**Migrácia grafu AAD**</span><span class="sxs-lookup"><span data-stu-id="8da07-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="8da07-125">V prípade aplikácií, ktoré používajú AAD Graph, postupujte podľa pokynov na migráciu aplikácie AAD Graph do programu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8da07-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="8da07-126">[Náš kontrolný zoznam migrácie poskytuje bod začiatku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="8da07-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="8da07-127">Na portáli registrácie aplikácie Azure sa zobrazuje, ktoré aplikácie používajú AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="8da07-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8da07-128">Odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a v prípade potreby osloviť nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="8da07-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8da07-129">Technická podpora spoločnosti Microsoft vám tiež poskytuje informácie o používaní AAD grafov v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="8da07-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







