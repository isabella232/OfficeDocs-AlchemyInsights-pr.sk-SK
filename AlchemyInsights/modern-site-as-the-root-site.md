---
title: Moderné lokalitu ako root
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232730"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="68036-102">Moderné lokalitu ako root</span><span class="sxs-lookup"><span data-stu-id="68036-102">Modern site as root site</span></span>

<span data-ttu-id="68036-103">My sme začali rollout novú funkciu, ktorá vám umožní vymeniť lokality klasické miesto koreňové s moderný web.</span><span class="sxs-lookup"><span data-stu-id="68036-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="68036-104">Pomocou [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie lokality s ďalším mieste počas archivácie pôvodnej lokality.</span><span class="sxs-lookup"><span data-stu-id="68036-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="68036-105">K dispozícii pre tím stránky (nie je pripojený k skupine) a komunikácie miesto.</span><span class="sxs-lookup"><span data-stu-id="68036-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="68036-106">Neodstraňujte klasickej koreňovej lokality vytvoriť lokalitu modernej komunikácie.</span><span class="sxs-lookup"><span data-stu-id="68036-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="68036-107">To nie je podporovaný spoločnosťou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="68036-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="68036-108">Odstránenie koreňovej lokality bude všetkých lokalít SharePoint vo vašej organizácii neprístupné pre všetkých užívateľov, kým obnovenie lokality alebo vytvoriť novú lokalitu na rovnakú adresu URL.</span><span class="sxs-lookup"><span data-stu-id="68036-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="68036-109">Sme bude komunikovať Táto funkcia cez centra správ.</span><span class="sxs-lookup"><span data-stu-id="68036-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="68036-110">By ste očakávať funkcie musia byť zapnuté v nájomcu krátko.</span><span class="sxs-lookup"><span data-stu-id="68036-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="68036-111">Známe problémy s vymieňania lokalít</span><span class="sxs-lookup"><span data-stu-id="68036-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="68036-112">Cieľová lokalita môže vrátiť "nebol nájdený" chyba (HTTP 404) za krátky čas.</span><span class="sxs-lookup"><span data-stu-id="68036-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="68036-113">Obsah bude musieť byť recrawled aktualizovať index vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="68036-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="68036-114">Neexistuje žiadny manuál krok vyžaduje tu, to sa deje automaticky.</span><span class="sxs-lookup"><span data-stu-id="68036-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="68036-115">Všetko závisí od "statické" odkazy (napríklad synchronizáciu súborov a OneNote súbory) treba manuálne opraviť.</span><span class="sxs-lookup"><span data-stu-id="68036-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="68036-116">Project Server lokality musí validovať zabezpečiť, že sú stále spojené správne.</span><span class="sxs-lookup"><span data-stu-id="68036-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
