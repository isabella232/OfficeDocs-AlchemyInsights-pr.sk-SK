---
title: Swap klasickej koreňovej lokality na modernú lokalitu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691194"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="f67c7-102">Swap klasickej koreňovej lokality na modernú lokalitu</span><span class="sxs-lookup"><span data-stu-id="f67c7-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="f67c7-103">Ak bolo vaše prostredie nastavené pred aprílom 2019, koreňovú lokalitu môžete zmeniť na modernú lokalitu pomocou prostredia Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f67c7-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="f67c7-104">Ak máte inú lokalitu, ktorú chcete použiť ako koreňovú lokalitu, môžete ju nahradiť [(vymeniť) koreňovú lokalitu](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="f67c7-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="f67c7-105">Pri archivácii pôvodnej lokality môžete použiť [vyvolanie-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) na výmenu umiestnenia lokality s inou lokalitou.</span><span class="sxs-lookup"><span data-stu-id="f67c7-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f67c7-106">K dispozícii pre tímovú lokalitu (nie je pripojená k skupine) a na komunikačnú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="f67c7-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="f67c7-107">Čoskoro sa dodajú ďalšie možnosti, ktoré vám umožnia naďalej používať obsah lokality, ale skonvertovať existujúcu lokalitu na komunikačnú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="f67c7-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="f67c7-108">Tieto možnosti sa budú postupne zavádzať.</span><span class="sxs-lookup"><span data-stu-id="f67c7-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="f67c7-109">Pokračujte v kontrole aktualizácií v centre správ.</span><span class="sxs-lookup"><span data-stu-id="f67c7-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f67c7-110">Známe problémy pri výmene lokalít</span><span class="sxs-lookup"><span data-stu-id="f67c7-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="f67c7-111">Cieľová lokalita môže počas krátkeho časového obdobia vrátiť chybu not found (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="f67c7-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f67c7-112">Ak chcete aktualizovať index vyhľadávania, bude potrebné prehľadať obsah.</span><span class="sxs-lookup"><span data-stu-id="f67c7-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f67c7-113">Nevyžaduje sa žiadny manuálny krok – tento postup sa vykoná automaticky.</span><span class="sxs-lookup"><span data-stu-id="f67c7-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="f67c7-114">Všetko, čo je závislé od statických prepojení (ako je napríklad synchronizácia súborov a OneNote), bude potrebné manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="f67c7-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f67c7-115">Ak je zdrojovou lokalitou lokalita na správu organizácie, aktualizujte URL adresu.</span><span class="sxs-lookup"><span data-stu-id="f67c7-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="f67c7-116">Získajte zoznam všetkých lokalít organizačných správ.</span><span class="sxs-lookup"><span data-stu-id="f67c7-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="f67c7-117">Lokality programu Project Server možno bude potrebné overiť, aby sa zabezpečilo, že sú stále priradení správne.</span><span class="sxs-lookup"><span data-stu-id="f67c7-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
