---
title: Moderná lokalita ako Koreňová lokalita
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666885"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="56b02-102">Moderná lokalita ako Koreňová lokalita</span><span class="sxs-lookup"><span data-stu-id="56b02-102">Modern site as root site</span></span>

<span data-ttu-id="56b02-103">Začali sme zavádzať novú funkciu, ktorá vám umožní [vymieňať si klasickú koreňovú lokalitu lokality s modernou lokalitou](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="56b02-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="56b02-104">Pri archivácii pôvodnej lokality môžete použiť [vyvolanie-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) na výmenu umiestnenia lokality s inou lokalitou.</span><span class="sxs-lookup"><span data-stu-id="56b02-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="56b02-105">K dispozícii pre tímovú lokalitu (nie je pripojená k skupine) a na komunikačnú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="56b02-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="56b02-106">Neodstraňujte klasickú koreňovú lokalitu a vytvorte modernú komunikačnú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="56b02-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="56b02-107">Spoločnosť Microsoft to nepodporuje.</span><span class="sxs-lookup"><span data-stu-id="56b02-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="56b02-108">Odstránením koreňovej lokality budú všetky lokality SharePoint vo vašej organizácii neprístupné pre všetkých používateľov, kým neobnovíte lokalitu alebo nevytvoríte novú lokalitu na rovnakej URL adrese.</span><span class="sxs-lookup"><span data-stu-id="56b02-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="56b02-109">Túto funkciu budeme komunikovať prostredníctvom centra správ.</span><span class="sxs-lookup"><span data-stu-id="56b02-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="56b02-110">V najbližšej dobe by ste mali očakávať, že funkcia bude v nájomníkovi zapnutá.</span><span class="sxs-lookup"><span data-stu-id="56b02-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="56b02-111">Známe problémy pri výmene lokalít</span><span class="sxs-lookup"><span data-stu-id="56b02-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="56b02-112">Cieľová lokalita môže počas krátkeho časového obdobia vrátiť chybu not found (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="56b02-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="56b02-113">Ak chcete aktualizovať index vyhľadávania, bude potrebné prehľadať obsah.</span><span class="sxs-lookup"><span data-stu-id="56b02-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="56b02-114">Tu nie je potrebný manuálny krok, tento postup sa vykoná automaticky.</span><span class="sxs-lookup"><span data-stu-id="56b02-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="56b02-115">Všetko, čo je závislé od statických prepojení (ako je napríklad synchronizácia súborov a OneNote), bude potrebné manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="56b02-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="56b02-116">Lokality programu Project Server možno bude potrebné overiť, aby sa zabezpečilo, že sú stále priradení správne.</span><span class="sxs-lookup"><span data-stu-id="56b02-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
