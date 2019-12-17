---
title: Problémy s výkonom-SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068432"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="66a57-102">SharePoint alebo OneDrive pomalé, nedostupné alebo nedostupné pre viacerých používateľov</span><span class="sxs-lookup"><span data-stu-id="66a57-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="66a57-103">SharePoint alebo OneDrive môže byť pomalé, nedostupné alebo nedostupné, alebo môže zobraziť službu nedostupné alebo 503 chyby, z niekoľkých dôvodov:</span><span class="sxs-lookup"><span data-stu-id="66a57-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="66a57-104">Ak je lokalita SharePoint alebo OneDrive pomalá alebo oneskorená pre viacerých používateľov, môže existovať dočasný problém so službou, pri ktorom používatelia vyskytnú občasné oneskorenia alebo chyby navigácie pri prístupe k lokalitám SharePoint alebo k obsahu OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="66a57-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="66a57-105">Ak chcete zistiť, či je vaša organizácia ovplyvnená, skontrolujte [stav služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="66a57-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="66a57-106">Používatelia môžu získať *503 server je zaneprázdnený* chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="66a57-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="66a57-107">Táto chyba môže byť spôsobená škrtenia v službe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="66a57-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="66a57-108">SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="66a57-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="66a57-109">Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="66a57-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="66a57-110">Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="66a57-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="66a57-111">Ak sa stretnete s pomalým výkonom s **klasickou** alebo **modernou** lokalitou alebo stránkou lokality SharePoint, využite [diagnostický nástroj stránky](https://aka.ms/perftool) na analýzu strán.</span><span class="sxs-lookup"><span data-stu-id="66a57-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="66a57-112">Ak stále skúsenosti všeobecné pomalý výkon, prečítajte si zdroje v spodnej časti tohto článku: [Úvod do ladenie výkonu pre SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="66a57-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  