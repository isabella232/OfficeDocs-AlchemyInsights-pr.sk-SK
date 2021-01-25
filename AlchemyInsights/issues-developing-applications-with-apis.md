---
title: Problémy s vývojom aplikácií pomocou rozhrania API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975017"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="7437d-102">Problémy s vývojom aplikácií pomocou rozhrania API</span><span class="sxs-lookup"><span data-stu-id="7437d-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="7437d-103">Ak chcete začať používať rozhranie API služby Azure Active Directory Graph, pozrite si príručku rozhrania API rýchlych reklám v službe [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) alebo zobrazenie [interaktívnej referenčnej dokumentácie rozhrania API služby Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="7437d-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="7437d-104">**Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="7437d-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7437d-105">**Od 30. júna 2020**, už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="7437d-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7437d-106">Budeme aj naďalej poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudú poskytovať aktualizácie funkcií.</span><span class="sxs-lookup"><span data-stu-id="7437d-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7437d-107">**Od 30. júna 2022**, ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="7437d-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7437d-108">Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však mať žiadne technické podpory ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="7437d-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="7437d-109">Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="7437d-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7437d-110">**Migrácia ADAL**</span><span class="sxs-lookup"><span data-stu-id="7437d-110">**ADAL Migration**</span></span>

<span data-ttu-id="7437d-111">Odporúčame aktualizovať na [knižnicu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="7437d-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7437d-112">Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií, aby MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z priebežných vylepšení zabezpečenia a funkcií MSAL.</span><span class="sxs-lookup"><span data-stu-id="7437d-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="7437d-113">[Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="7437d-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7437d-114">[Zistite, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="7437d-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7437d-115">Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť všetkých nezávislých poskytovateľov služieb alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="7437d-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7437d-116">Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií, ktoré nie sú Microsoft ADAL v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="7437d-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7437d-117">**Migrácia grafu AAD**</span><span class="sxs-lookup"><span data-stu-id="7437d-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="7437d-118">V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa pokynov na migráciu [aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7437d-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="7437d-119">[Náš kontrolný zoznam migrácie poskytuje bod začiatku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="7437d-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="7437d-120">Na portáli registrácie aplikácie Azure sa zobrazuje, ktoré aplikácie používajú AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7437d-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7437d-121">Odporúčame, aby ste si prečítali všetky zdrojové kódy aplikácií a ak je to možné, Oslovte ľubovoľných poskytovateľov ISV alebo aplikácií.</span><span class="sxs-lookup"><span data-stu-id="7437d-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7437d-122">Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití AAD grafov v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="7437d-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="7437d-123">Pre aplikáciu na prístup k údajom v programe Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu.</span><span class="sxs-lookup"><span data-stu-id="7437d-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7437d-124">V [odkaze na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) sú uvedené povolenia priradené k jednotlivým hlavným množinám rozhraní API programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7437d-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7437d-125">Poskytuje aj usmernenie o tom, ako používať povolenia.</span><span class="sxs-lookup"><span data-stu-id="7437d-125">It also provides guidance about how to use the permissions.</span></span>
