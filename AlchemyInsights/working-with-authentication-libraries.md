---
title: Práca s knižnicami na overovanie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036869"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="90261-102">Práca s knižnicami na overovanie</span><span class="sxs-lookup"><span data-stu-id="90261-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="90261-103">Ak chcete vyriešiť problém s knižnicou Microsoft Authentication Library (MSAL), vykonajte tieto Odporúčané kroky:</span><span class="sxs-lookup"><span data-stu-id="90261-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="90261-104">**Práca s MSAL**: [knižnice overovania platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – v tomto článku sa zobrazuje podpora knižnice Microsoft Authentication Library pre viacero typov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="90261-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="90261-105">Obsahuje prepojenia na zdrojový kód knižnice. kde získate balík pre projekt vašej aplikácie, a či knižnica podporuje prihlásenie používateľa (overenie), prístup k zabezpečeným webovým rozhraniam API (autorizácia) alebo obom.</span><span class="sxs-lookup"><span data-stu-id="90261-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="90261-106">**Riešenie problémov s overovaním**: MSAL podporuje viacero tokov overovania, ktoré sa používajú v rôznych scenároch aplikácie.</span><span class="sxs-lookup"><span data-stu-id="90261-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="90261-107">V závislosti od toho, ako je vaša klientska aplikácia vytvorená, môže MSAL použiť jeden alebo viacero overovacích tokov podporovaných platformou Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="90261-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="90261-108">Tieto toky môžu produkovať niekoľko typov tokenov a autorizačných kódov a vyžadovať rôzne tokeny, aby mohli pracovať.</span><span class="sxs-lookup"><span data-stu-id="90261-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="90261-109">**Prístupové tokeny**: [tokeny prístupu k platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Zistite, ako môže vaše rozhranie API overiť a použiť nároky v accessovom tokene.</span><span class="sxs-lookup"><span data-stu-id="90261-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="90261-110">Celá dokumentácia v tomto článku s výnimkou prípadov, keď je uvedené, sa vzťahuje len na tokeny vydané pre rozhrania API, ktoré ste zaregistrovali.</span><span class="sxs-lookup"><span data-stu-id="90261-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="90261-111">Nevzťahuje sa na tokeny vydané pre rozhrania API vo vlastníctve spoločnosti Microsoft a nie je možné použiť tieto tokeny na overenie, akým spôsobom bude platforma Microsoft Identity vydávať tokeny pre vytvorené API.</span><span class="sxs-lookup"><span data-stu-id="90261-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="90261-112">**Ukončenie podpory pre knižnicu overovania služby Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="90261-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="90261-113">**Od 30. júna 2020,** už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="90261-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="90261-114">Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.</span><span class="sxs-lookup"><span data-stu-id="90261-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="90261-115">**Od 30. júna 2022,** ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="90261-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="90261-116">Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však *mať žiadne technické podpory ani aktualizácie zabezpečenia*.</span><span class="sxs-lookup"><span data-stu-id="90261-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="90261-117">Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="90261-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="90261-118">**Migrácia ADAL**</span><span class="sxs-lookup"><span data-stu-id="90261-118">**ADAL Migration**</span></span>

- <span data-ttu-id="90261-119">Odporúčame aktualizáciu na MSAL, ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="90261-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="90261-120">Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií do MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z priebežných vylepšení zabezpečenia a funkcií MSAL.</span><span class="sxs-lookup"><span data-stu-id="90261-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="90261-121">[Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="90261-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="90261-122">[Zistite, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="90261-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="90261-123">Ak po prečítaní príručky pre platformu aplikácie máte ďalšie otázky, môžete uverejniť príspevok na [lokalite Microsoft Q&a](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) so značkou [Azure-AD-ADAL-odmietanie] alebo otvoriť problém v úložisku GitHub knižnice.</span><span class="sxs-lookup"><span data-stu-id="90261-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="90261-124">Pozrite si časť [jazyky a rámce](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) v článku **Prehľad MSAL** pre prepojenia na repo služby jednotlivých knižníc.</span><span class="sxs-lookup"><span data-stu-id="90261-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="90261-125">**Ak potrebujete pomôcť s pochopením, ktoré z vašich aplikácií používajú ADAL**, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií.</span><span class="sxs-lookup"><span data-stu-id="90261-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="90261-126">Ak je to možné, Oslovte všetkých nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií.</span><span class="sxs-lookup"><span data-stu-id="90261-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="90261-127">Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="90261-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







