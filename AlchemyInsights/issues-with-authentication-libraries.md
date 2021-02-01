---
title: Problémy s overovaním knižníc
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063644"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="44cf2-102">Problémy s overovaním knižníc</span><span class="sxs-lookup"><span data-stu-id="44cf2-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="44cf2-103">[Knižnice overovania platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) sú uvedené v zoznamoch knižníc podporovaných spoločnosťou Microsoft a kompatibilných klientskych a middleware knižníc.</span><span class="sxs-lookup"><span data-stu-id="44cf2-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="44cf2-104">Knižnica Microsoft Authentication Library (MSAL) podporuje viacero [tokov overovania](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , ktoré sa používajú v rôznych scenároch aplikácie.</span><span class="sxs-lookup"><span data-stu-id="44cf2-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="44cf2-105">Ak chcete overiť a získať tokeny, môžete v kóde inicializovať novú verejnú alebo dôvernú klientsku aplikáciu.</span><span class="sxs-lookup"><span data-stu-id="44cf2-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="44cf2-106">Pri inicializácii klientskej aplikácie v knižnici Microsoft Authentication Library (MSAL) môžete nastaviť niekoľko možností konfigurácie.</span><span class="sxs-lookup"><span data-stu-id="44cf2-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="44cf2-107">Ďalšie informácie nájdete v téme [možnosti konfigurácie aplikácie](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="44cf2-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="44cf2-108">**Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="44cf2-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="44cf2-109">**Od 30. júna 2020**, už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="44cf2-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="44cf2-110">Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.</span><span class="sxs-lookup"><span data-stu-id="44cf2-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="44cf2-111">**Od 30. júna 2022**, ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="44cf2-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="44cf2-112">Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však *mať žiadne technické podpory ani aktualizácie zabezpečenia*.</span><span class="sxs-lookup"><span data-stu-id="44cf2-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="44cf2-113">Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="44cf2-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="44cf2-114">**Migrácia ADAL**</span><span class="sxs-lookup"><span data-stu-id="44cf2-114">**ADAL Migration**</span></span>

<span data-ttu-id="44cf2-115">Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="44cf2-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="44cf2-116">Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií, aby MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z pokračujúcich funkcií zabezpečenia a vylepšení MSAL.</span><span class="sxs-lookup"><span data-stu-id="44cf2-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="44cf2-117">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="44cf2-117">For more information, see:</span></span>

1. [<span data-ttu-id="44cf2-118">Prečítajte si najčastejšie otázky o ADAL</span><span class="sxs-lookup"><span data-stu-id="44cf2-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="44cf2-119">Informácie o migrácii aplikácií na platforme</span><span class="sxs-lookup"><span data-stu-id="44cf2-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="44cf2-120">Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť všetkých nezávislých poskytovateľov služieb alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="44cf2-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="44cf2-121">Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44cf2-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="44cf2-122">**Migrácia AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="44cf2-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="44cf2-123">V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa pokynov na [migráciu aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="44cf2-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="44cf2-124">Náš kontrolný zoznam migrácie poskytuje bod začiatku.</span><span class="sxs-lookup"><span data-stu-id="44cf2-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="44cf2-125">Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="44cf2-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="44cf2-126">Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="44cf2-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="44cf2-127">Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití AAD grafov v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="44cf2-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="44cf2-128">Pre aplikáciu na prístup k údajom v programe Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu.</span><span class="sxs-lookup"><span data-stu-id="44cf2-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="44cf2-129">V [odkaze na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sú uvedené povolenia priradené k jednotlivým hlavným množinám rozhraní API programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="44cf2-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="44cf2-130">Poskytuje aj usmernenie o tom, ako používať povolenia.</span><span class="sxs-lookup"><span data-stu-id="44cf2-130">It also provides guidance about how to use the permissions.</span></span>
