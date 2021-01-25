---
title: Dotazovanie rozhrania API programu Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974685"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="8736e-102">Dotazovanie rozhrania API programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="8736e-103">Táto téma sa môže vzťahovať aj na vývojárov, ktorí stále používajú rozhranie API služby Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="8736e-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="8736e-104">**Dôrazne** sa však odporúča používať program Microsoft Graph na všetky scenáre v adresári, identite a Accesse.</span><span class="sxs-lookup"><span data-stu-id="8736e-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="8736e-105">**Problémy s overovaním alebo autorizáciou**</span><span class="sxs-lookup"><span data-stu-id="8736e-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="8736e-106">Ak vaša aplikácia **nedokáže získať tokeny** na volanie do programu Microsoft Graph, vyberte **problém s použitím kategórie accessových tokenov (Authentication)** pre Microsoft Graph a získajte konkrétnu pomoc a podporu v tejto téme.</span><span class="sxs-lookup"><span data-stu-id="8736e-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="8736e-107">Ak vaša aplikácia **prijíma chyby autorizácie 401 alebo 403** pri volaní programu Microsoft Graph, vyberte položku **získať chybu odmietnutia prístupu (autorizácia)** Microsoft Graphu API, aby ste získali konkrétnu pomoc a podporu v tejto téme.</span><span class="sxs-lookup"><span data-stu-id="8736e-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="8736e-108">**Chcem použiť Microsoft Graph, ale nie ste si istí, kde začať**</span><span class="sxs-lookup"><span data-stu-id="8736e-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="8736e-109">Ďalšie informácie o programe Microsoft Graph nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="8736e-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="8736e-110">Prehľad programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="8736e-111">Prehľad identity a riadenia prístupu v programe Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="8736e-112">Začíname s budovaním aplikácií Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="8736e-113">**Microsoft Graph Explorer** – testovanie API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi</span><span class="sxs-lookup"><span data-stu-id="8736e-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="8736e-114">**Chcem používať Microsoft Graph, ale podporuje to rozhrania v 1.0 Directory API, ktoré potrebujem?**</span><span class="sxs-lookup"><span data-stu-id="8736e-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="8736e-115">Microsoft Graph je odporúčaný API pre adresár, identitu a riadenie prístupu.</span><span class="sxs-lookup"><span data-stu-id="8736e-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="8736e-116">Existuje však niekoľko rozdielov medzi tým, čo je možné v službe Azure AD Graph a Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8736e-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="8736e-117">Pozrite si nasledujúce články, ktoré zvýrazňujú najaktuálnejšie rozdiely na pomoc pri výbere:</span><span class="sxs-lookup"><span data-stu-id="8736e-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="8736e-118">Rozdiely v type zdroja medzi Azure AD Graph a Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="8736e-119">Rozdiely medzi vlastnosťami medzi Azure AD Graphom a Microsoft Graphom</span><span class="sxs-lookup"><span data-stu-id="8736e-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="8736e-120">Rozdiely v metóde medzi službou Azure AD a programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="8736e-121">**Pri dotaze na objekt *používateľa* chýbajú mnohé z jeho vlastností**</span><span class="sxs-lookup"><span data-stu-id="8736e-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="8736e-122">`GET https://graph.microsoft.com/v1.0/users` vráti iba 11 vlastností, pretože Microsoft Graph automaticky vyberie predvolenú množinu vlastností *používateľa* , ktorá sa má vrátiť.</span><span class="sxs-lookup"><span data-stu-id="8736e-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="8736e-123">Ak potrebujete ďalšie vlastnosti *používateľa* , použite $Select na výber vlastností, ktoré potrebuje vaša aplikácia.</span><span class="sxs-lookup"><span data-stu-id="8736e-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="8736e-124">Vyskúšajte si to v **programe Microsoft Graph Explorer** ako prvý.</span><span class="sxs-lookup"><span data-stu-id="8736e-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="8736e-125">**Niektoré hodnoty vlastností používateľa majú *hodnotu null* , aj keď viem, že sú nastavené**</span><span class="sxs-lookup"><span data-stu-id="8736e-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="8736e-126">Najpravdepodobnejšie vysvetlenie je, že žiadosť bola poskytnutá *používateľovi. ReadBasic. All* permission.</span><span class="sxs-lookup"><span data-stu-id="8736e-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="8736e-127">To umožňuje aplikácii čítať obmedzenú množinu vlastností používateľa a vrátiť všetky ostatné vlastnosti ako hodnotu null aj v prípade, že boli predtým nastavené.</span><span class="sxs-lookup"><span data-stu-id="8736e-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="8736e-128">Skúste udeliť používateľovi aplikácie *. read. All* povolenie namiesto toho.</span><span class="sxs-lookup"><span data-stu-id="8736e-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="8736e-129">Ďalšie informácie nájdete v téme [povolenia používateľov programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="8736e-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="8736e-130">**Mám problémy s používaním parametrov dotazu OData na filtrovanie údajov v mojich požiadavkách**</span><span class="sxs-lookup"><span data-stu-id="8736e-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="8736e-131">Zatiaľ čo Microsoft Graph podporuje širokú škálu parametrov OData dotazu, mnohé z týchto parametrov nie sú plne podporované v adresárových službách (zdroje, ktoré dedia z *directoryObject*) v Microsoft graphe.</span><span class="sxs-lookup"><span data-stu-id="8736e-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="8736e-132">Rovnaké obmedzenia, ktoré boli prítomné v službe Azure AD Graphu, sú v Microsoft Graphe naďalej z veľkej časti:</span><span class="sxs-lookup"><span data-stu-id="8736e-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="8736e-133">**Nepodporované**: $count, $search a $filter s hodnotami *null* alebo *NOT NULL*</span><span class="sxs-lookup"><span data-stu-id="8736e-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="8736e-134">**Nie je podporované**: $filter na niektoré vlastnosti (pozrite tému zdroje informácií o tom, ktoré vlastnosti sú filtrované)</span><span class="sxs-lookup"><span data-stu-id="8736e-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="8736e-135">**Nepodporované**: stránkovanie, filtrovanie a zoraďovanie súčasne</span><span class="sxs-lookup"><span data-stu-id="8736e-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="8736e-136">**Nie je podporované**: filtrovanie vzťahu.</span><span class="sxs-lookup"><span data-stu-id="8736e-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="8736e-137">Napríklad – vyhľadanie všetkých členov inžinierskej skupiny, ktoré sú vo Veľkej Británii.</span><span class="sxs-lookup"><span data-stu-id="8736e-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="8736e-138">**Čiastočná podpora**: $orderby na *používateľa* (iba DisplayName a userPrincipalName) a *skupina*</span><span class="sxs-lookup"><span data-stu-id="8736e-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="8736e-139">**Čiastočná podpora**: $filter (podporuje iba *EQ*, startswith *alebo*, *a* *a Limited)* podporu, $Expand (rozšírenie vzťahov jedného objektu vráti všetky vzťahy, ale rozšírenie skupiny vzťahov objektov je obmedzené) </span><span class="sxs-lookup"><span data-stu-id="8736e-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="8736e-140">Ďalšie informácie nájdete v téme [Prispôsobenie odpovedí pomocou parametrov dotazu](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8736e-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="8736e-141">**Volanie rozhrania API nefunguje – kde môžem vykonať ďalšie testovanie?**</span><span class="sxs-lookup"><span data-stu-id="8736e-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="8736e-142">**Microsoft Graph Explorer** – otestujte rozhrania API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi a pozrite si aj **vzorové dotazy** v programe Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="8736e-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="8736e-143">**Pri dotaze na údaje sa zdá, že je naspäť neúplný súbor údajov**</span><span class="sxs-lookup"><span data-stu-id="8736e-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="8736e-144">Ak vytvárate dotaz na kolekciu (napríklad *Používatelia*), Microsoft Graph použije limity stránok na strane servera, takže výsledky sa vždy vrátia s predvolenou veľkosťou strany.</span><span class="sxs-lookup"><span data-stu-id="8736e-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="8736e-145">Vaša aplikácia by mala vždy očakávať, že prejdete na stránku prostredníctvom kolekcií vrátených zo služby.</span><span class="sxs-lookup"><span data-stu-id="8736e-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="8736e-146">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="8736e-146">For more information, see:</span></span>

- [<span data-ttu-id="8736e-147">Najvhodnejšie postupy v programe Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="8736e-148">Stránkovanie údajov programu Microsoft Graph v aplikácii</span><span class="sxs-lookup"><span data-stu-id="8736e-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="8736e-149">**Moja aplikácia je príliš pomalá a je tiež stále obmedzovaná. Aké vylepšenia môžem urobiť?**</span><span class="sxs-lookup"><span data-stu-id="8736e-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="8736e-150">V závislosti od vášho scenára je k dispozícii široká škála rôznych možností, ktoré vám pomôžu vykonať viac výkonných aplikácií a v niektorých prípadoch menej náchylné na obmedzovanie službou (pri príliš veľkom počte hovorov).</span><span class="sxs-lookup"><span data-stu-id="8736e-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="8736e-151">Ďalšie informácie nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="8736e-151">To learn more, see:</span></span>

- [<span data-ttu-id="8736e-152">Najvhodnejšie postupy v programe Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="8736e-153">Požiadavky na dávkovanie</span><span class="sxs-lookup"><span data-stu-id="8736e-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="8736e-154">Sledovanie zmien prostredníctvom Delta dotazu</span><span class="sxs-lookup"><span data-stu-id="8736e-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="8736e-155">Upozornenia na zmeny prostredníctvom webhookov</span><span class="sxs-lookup"><span data-stu-id="8736e-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="8736e-156">Usmernenie o obmedzovaní</span><span class="sxs-lookup"><span data-stu-id="8736e-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="8736e-157">**Kde nájdem ďalšie informácie o chybách a známych problémoch?**</span><span class="sxs-lookup"><span data-stu-id="8736e-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="8736e-158">Informácie o odpovedaní na chyby v Microsoft Graphe</span><span class="sxs-lookup"><span data-stu-id="8736e-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="8736e-159">Známe problémy s aplikáciou Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8736e-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="8736e-160">**Kde môžem skontrolovať stav dostupnosti a pripojenia služby?**</span><span class="sxs-lookup"><span data-stu-id="8736e-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="8736e-161">Dostupnosť služieb a pripojenie k základným službám, ku ktorým je možné získať prístup prostredníctvom programu Microsoft Graph, môže mať vplyv na celkovú dostupnosť a výkon programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8736e-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="8736e-162">Ak ide o stav služby Azure Active Directory, pozrite si stav služieb **zabezpečenia a identít** uvedených na [stránke stavu Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="8736e-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="8736e-163">V prípade služieb Office, ktoré prispievajú do programu Microsoft Graph, skontrolujte stav služieb uvedených v časti [Tabuľa stavu služieb balíka Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8736e-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
