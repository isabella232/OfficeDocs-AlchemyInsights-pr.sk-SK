---
title: Moderné stránky ako koreňovej stránky
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054717"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0ee13-102">Moderné stránky ako root site</span><span class="sxs-lookup"><span data-stu-id="0ee13-102">Modern site as root site</span></span>

<span data-ttu-id="0ee13-103">Začali sme zavádzanie novej funkcie, ktorá vám umožní [vymeniť klasické stránky koreňovej stránky s moderným mieste](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="0ee13-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="0ee13-104">Použitie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie stránky s inou lokalitou pri archivácii pôvodnej stránky.</span><span class="sxs-lookup"><span data-stu-id="0ee13-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0ee13-105">K dispozícii pre obe tímové stránky (nie je pripojený k skupine) a komunikačné stránky.</span><span class="sxs-lookup"><span data-stu-id="0ee13-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="0ee13-106">Neodstraňujte svoju klasickú koreňovú stránku na vytvorenie modernej komunikačnej stránky.</span><span class="sxs-lookup"><span data-stu-id="0ee13-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0ee13-107">Toto nie je podporovaný spoločnosťou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0ee13-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="0ee13-108">Odstránením koreňovej lokality sa všetky lokality SharePoint vo vašej organizácii neprístupné všetkým používateľom, kým neobnovíte lokalitu alebo vytvoríte novú lokalitu na rovnakej adrese URL.</span><span class="sxs-lookup"><span data-stu-id="0ee13-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="0ee13-109">Túto funkciu budeme komunikovať prostredníctvom centra správ.</span><span class="sxs-lookup"><span data-stu-id="0ee13-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="0ee13-110">Mali by ste očakávať, že funkcia bude zapnutá v nájomcovi krátko.</span><span class="sxs-lookup"><span data-stu-id="0ee13-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0ee13-111">Známe problémy s vymenením lokalít</span><span class="sxs-lookup"><span data-stu-id="0ee13-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="0ee13-112">Cieľová lokalita môže vrátiť chybu "Not Found" (HTTP 404) na krátku dobu.</span><span class="sxs-lookup"><span data-stu-id="0ee13-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0ee13-113">Obsah bude musieť byť recrawled aktualizovať vyhľadávací index.</span><span class="sxs-lookup"><span data-stu-id="0ee13-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0ee13-114">Neexistuje žiadny manuálny krok vyžaduje tu, to bude vykonané automaticky.</span><span class="sxs-lookup"><span data-stu-id="0ee13-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="0ee13-115">Čokoľvek závislé na "statické" odkazy (napríklad synchronizácia súborov a súbory programu OneNote) bude potrebné manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="0ee13-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0ee13-116">Lokality Project Server môže byť potrebné overiť, aby sa zabezpečilo, že sú stále spojené správne.</span><span class="sxs-lookup"><span data-stu-id="0ee13-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
