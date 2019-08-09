---
title: Swap vaše klasickej koreňovej lokality s moderný web
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270759"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="6bf52-102">Swap vaše klasickej koreňovej lokality s moderný web</span><span class="sxs-lookup"><span data-stu-id="6bf52-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="6bf52-103">Ak vaše prostredie bola zriadená pred máj 2019, môžete zmeniť koreňovou lokalitou na moderné stránky pomocou Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6bf52-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="6bf52-104">Ak máte rôzne stránky, ktoré chcete použiť ako koreňovú lokalitu, môžete nahradiť (swap) koreň mieste s ním.</span><span class="sxs-lookup"><span data-stu-id="6bf52-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="6bf52-105">Pomocou [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie lokality s ďalším mieste počas archivácie pôvodnej lokality.</span><span class="sxs-lookup"><span data-stu-id="6bf52-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6bf52-106">K dispozícii pre tím stránky (nie je pripojený k skupine) a komunikácie miesto.</span><span class="sxs-lookup"><span data-stu-id="6bf52-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="6bf52-107">Ďalšie možnosti budú zavedené čoskoro ktoré vám umožní používať obsah na webe, ale prevod existujúcej lokality na lokalitu komunikácie.</span><span class="sxs-lookup"><span data-stu-id="6bf52-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="6bf52-108">Tieto schopnosti bude postupne váľa.</span><span class="sxs-lookup"><span data-stu-id="6bf52-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="6bf52-109">Pokračovať v kontrole stredisku správ v Office 365 aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="6bf52-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6bf52-110">Známe problémy s vymieňania lokalít</span><span class="sxs-lookup"><span data-stu-id="6bf52-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="6bf52-111">Cieľová lokalita môže vrátiť "nebol nájdený" chyba (HTTP 404) za krátky čas.</span><span class="sxs-lookup"><span data-stu-id="6bf52-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6bf52-112">Obsah bude musieť byť recrawled aktualizovať index vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="6bf52-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6bf52-113">Neexistuje žiadny manuál krok potrebný - to sa deje automaticky.</span><span class="sxs-lookup"><span data-stu-id="6bf52-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="6bf52-114">Všetko závisí od "statické" odkazy (napríklad synchronizáciu súborov a OneNote súbory) treba manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="6bf52-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6bf52-115">Ak zdroj stránky bolo organizačné Novinky stránok, aktualizácia URL.</span><span class="sxs-lookup"><span data-stu-id="6bf52-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="6bf52-116">Získajte zoznam všetkých organizačných spravodajských webov.</span><span class="sxs-lookup"><span data-stu-id="6bf52-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="6bf52-117">Project Server lokality musí validovať zabezpečiť, že sú stále spojené správne.</span><span class="sxs-lookup"><span data-stu-id="6bf52-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





