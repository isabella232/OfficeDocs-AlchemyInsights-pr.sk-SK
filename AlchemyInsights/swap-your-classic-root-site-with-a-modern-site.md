---
title: Swap klasickej koreňovej stránky s moderným mieste
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741559"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="09860-102">Swap klasickej koreňovej stránky s moderným mieste</span><span class="sxs-lookup"><span data-stu-id="09860-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="09860-103">Ak bolo vaše prostredie nastavené pred aprílom 2019, môžete zmeniť koreňovú lokalitu na modernú lokalitu pomocou prostredia Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="09860-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="09860-104">Ak máte inú lokalitu, ktorú chcete použiť ako svoju koreňovú lokalitu, môžete s ňou nahradiť [(vymeniť) koreňovú lokalitu](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="09860-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="09860-105">Použitie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie stránky s inou lokalitou pri archivácii pôvodnej stránky.</span><span class="sxs-lookup"><span data-stu-id="09860-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="09860-106">K dispozícii pre obe tímové stránky (nie je pripojený k skupine) a komunikačné stránky.</span><span class="sxs-lookup"><span data-stu-id="09860-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="09860-107">Ďalšie možnosti budú predstavené čoskoro, že vám umožní udržať používanie obsahu na webe, ale previesť existujúce stránky na komunikačné miesto.</span><span class="sxs-lookup"><span data-stu-id="09860-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="09860-108">Tieto schopnosti budú postupne váľa.</span><span class="sxs-lookup"><span data-stu-id="09860-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="09860-109">Pokračujte v kontrole aktualizácií centra správ.</span><span class="sxs-lookup"><span data-stu-id="09860-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="09860-110">Známe problémy s vymenením lokalít</span><span class="sxs-lookup"><span data-stu-id="09860-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="09860-111">Cieľová lokalita môže vrátiť chybu "Not Found" (HTTP 404) na krátku dobu.</span><span class="sxs-lookup"><span data-stu-id="09860-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="09860-112">Obsah bude musieť byť recrawled aktualizovať vyhľadávací index.</span><span class="sxs-lookup"><span data-stu-id="09860-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="09860-113">Nie je potrebný manuálny krok-to bude vykonané automaticky.</span><span class="sxs-lookup"><span data-stu-id="09860-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="09860-114">Čokoľvek závislé na "statické" odkazy (napríklad synchronizácia súborov a súbory programu OneNote) bude potrebné manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="09860-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="09860-115">Ak zdrojová lokalita bola lokalita správy organizácie, aktualizujte adresu URL.</span><span class="sxs-lookup"><span data-stu-id="09860-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="09860-116">Získajte zoznam všetkých organizačných spravodajských webov.</span><span class="sxs-lookup"><span data-stu-id="09860-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="09860-117">Lokality Project Server môže byť potrebné overiť, aby sa zabezpečilo, že sú stále spojené správne.</span><span class="sxs-lookup"><span data-stu-id="09860-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
