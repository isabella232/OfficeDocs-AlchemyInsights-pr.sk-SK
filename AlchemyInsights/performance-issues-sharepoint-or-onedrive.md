---
title: Problémy s výkonom – SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771916"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="32fe6-102">Služby SharePoint alebo OneDrive sú pomalé, nedostupné alebo nie sú k dispozícii pre viacerých používateľov</span><span class="sxs-lookup"><span data-stu-id="32fe6-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="32fe6-103">SharePoint alebo OneDrive môže byť pomalý, nedostupný alebo nedostupný alebo môže zobraziť služby nedostupné alebo 503 chyby z niekoľkých dôvodov:</span><span class="sxs-lookup"><span data-stu-id="32fe6-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="32fe6-104">Ak je lokalita SharePoint alebo OneDrive v prípade viacerých používateľov pomalá alebo oneskorená, môže sa vyskytnúť dočasný problém so službou, v ktorom používatelia vyskytnú občasné oneskorenia alebo chyby navigácie pri prístupe k lokalitám SharePoint alebo k obsahu OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="32fe6-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="32fe6-105">Ak chcete zistiť, či je vaša organizácia ovplyvnená, pozrite si [tabuľu stavu služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="32fe6-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="32fe6-106">Pri pokuse o prechod na lokalitu SharePoint alebo OneDrive môžu používatelia získať *server 503 je zaneprázdnená* chyba.</span><span class="sxs-lookup"><span data-stu-id="32fe6-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="32fe6-107">Táto chyba môže byť spôsobená obmedzovaním v rámci služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32fe6-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="32fe6-108">SharePoint Online používa obmedzovanie na udržiavanie optimálneho výkonu a spoľahlivosti služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="32fe6-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="32fe6-109">Obmedzovanie zníži počet akcií používateľa alebo súbežných hovorov (podľa skriptu alebo kódu), aby sa zabránilo nadužívanie zdrojov.</span><span class="sxs-lookup"><span data-stu-id="32fe6-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="32fe6-110">Ďalšie informácie o obmedzovaní nájdete v téme [zamedzenie obmedzovania alebo blokovania v SharePointe Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="32fe6-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="32fe6-111">Ak sa stretnete s pomalým výkonom s **klasickou** alebo **modernou** lokalitou alebo stránkou SharePointu, využite [nástroj na diagnostiku stránky](https://aka.ms/perftool) na analýzu stránok.</span><span class="sxs-lookup"><span data-stu-id="32fe6-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="32fe6-112">Ak sa stále vyskytuje všeobecný pomalý výkon, pozrite si zdroje v spodnej časti tohto článku: [úvodné informácie o ladení výkonu pre SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="32fe6-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  