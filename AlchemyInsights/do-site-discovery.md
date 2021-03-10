---
title: Zisťovanie lokality
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694558"
---
# <a name="do-site-discovery"></a><span data-ttu-id="d7e98-102">Zisťovanie lokality</span><span class="sxs-lookup"><span data-stu-id="d7e98-102">Do site discovery</span></span>

<span data-ttu-id="d7e98-103">Ak vaša organizácia stále používa staršie webové aplikácie a plány na používanie režimu Internet Explorer (ktoré väčšina zákazníkov robí), mali by ste vykonať ďalšie vyhľadávanie lokalít.</span><span class="sxs-lookup"><span data-stu-id="d7e98-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="d7e98-104">**Už ste nasadili staršiu verziu prehliadača Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="d7e98-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="d7e98-105">Ak ste už zoznam podnikových lokalít nakonfigurovali tak, aby fungoval pre staršiu verziu prehliadača Microsoft Edge, zisťovanie lokality je takmer hotové.</span><span class="sxs-lookup"><span data-stu-id="d7e98-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="d7e98-106">Je možné, že je potrebné pridať neutrálne lokality.</span><span class="sxs-lookup"><span data-stu-id="d7e98-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="d7e98-107">Neutrálne lokality sú zvyčajne lokality, ktoré poskytujú jediné prihlásenie (SSO).</span><span class="sxs-lookup"><span data-stu-id="d7e98-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="d7e98-108">Ak prejdete na neutrálne miesto v prehliadači Microsoft Edge, potom sa chcete vrátiť do prehliadača Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d7e98-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="d7e98-109">Ak prejdete na neutrálnu lokalitu v režime Internet Explorer, v režime Internet Explorer sa chcete overiť.</span><span class="sxs-lookup"><span data-stu-id="d7e98-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="d7e98-110">Identifikujte všetky SSO alebo iné neutrálne lokality, ktoré používate, a pridajte ich do zoznamu podnikových lokalít.</span><span class="sxs-lookup"><span data-stu-id="d7e98-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="d7e98-111">**Internet Explorer je predvoleným prehliadačom**</span><span class="sxs-lookup"><span data-stu-id="d7e98-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="d7e98-112">Ak teraz používate Internet Explorer, možno neviete, ktoré lokality boli inovované na moderné webové štandardy a ktoré stále vyžadujú Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d7e98-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="d7e98-113">Tieto lokality budete chcieť nájsť a pridať do zoznamu podnikových lokalít, aby ste mohli používať režim Internet Explorera len pre tieto lokality.</span><span class="sxs-lookup"><span data-stu-id="d7e98-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="d7e98-114">[Zisťovanie podnikovej lokality](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) zistí lokality, ktoré môžu potrebovať režim programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d7e98-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="d7e98-115">Môže zhromažďovať údaje v počítačoch s Windowsom Internet Explorerom 8 cez Internet Explorer 11 vo Windowse 10, Windowse 8,1 alebo Windowse 7.</span><span class="sxs-lookup"><span data-stu-id="d7e98-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="d7e98-116">**Analýza údajov**</span><span class="sxs-lookup"><span data-stu-id="d7e98-116">**Analyze the data**</span></span>

<span data-ttu-id="d7e98-117">Po zhromaždení údajov lokality odporúčame, aby ste údaje analyzovali nasledujúcim procesom:</span><span class="sxs-lookup"><span data-stu-id="d7e98-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="d7e98-118">Zoraďte údaje podľa domény a potom podľa URL adresy.</span><span class="sxs-lookup"><span data-stu-id="d7e98-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="d7e98-119">Definujte hranice aplikácie, ktorá sa má konfigurovať v režime Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d7e98-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="d7e98-120">Chcete zahrnúť všetky lokality a webové ovládacie prvky, ktoré definujú aplikáciu, ale nechcete zahrnúť ďalšie lokality a ovládacie prvky.</span><span class="sxs-lookup"><span data-stu-id="d7e98-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="d7e98-121">Niektoré lokality môžu byť jednoduché, pretože *https://contoso.com/app1* iné môžu vyžadovať definovanie viacerých lokalít a stránok.</span><span class="sxs-lookup"><span data-stu-id="d7e98-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="d7e98-122">Otestujte aplikáciu a overte, či nefungovala natívne.</span><span class="sxs-lookup"><span data-stu-id="d7e98-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="d7e98-123">Mnoho lokalít ponúkne moderný obsah pri zisťovaní moderného prehliadača a ponúka iba starší obsah pri zisťovaní programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d7e98-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="d7e98-124">Ak zlyhá testovanie, pridajte aplikáciu do zoznamu podnikových lokalít.</span><span class="sxs-lookup"><span data-stu-id="d7e98-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="d7e98-125">Ako najvhodnejší postup sa zoskupujú všetky lokality, ktoré obsahujú aplikáciu.</span><span class="sxs-lookup"><span data-stu-id="d7e98-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="d7e98-126">Týmto spôsobom je pri inovácii aplikácie jednoduchšie odstrániť celú lokalitu z režimu Internet Explorer a začať používať moderný prehliadač pre danú aplikáciu.</span><span class="sxs-lookup"><span data-stu-id="d7e98-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="d7e98-127">Po dokončení vyhľadávania lokality a analyzovaní údajov môžete začať pozerať na svoju stratégiu kanála.</span><span class="sxs-lookup"><span data-stu-id="d7e98-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

