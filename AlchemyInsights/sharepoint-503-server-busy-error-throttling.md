---
title: SharePoint Online obmedzovanie
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742224"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="57339-102">SharePoint Online obmedzovanie</span><span class="sxs-lookup"><span data-stu-id="57339-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="57339-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="57339-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="57339-104">**503 server je zaneprázdnený chyba**</span><span class="sxs-lookup"><span data-stu-id="57339-104">**503 server is busy error**</span></span>

<span data-ttu-id="57339-105">Používatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="57339-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="57339-106">Táto chyba môže byť spôsobená škrtenia v službe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57339-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="57339-107">SharePoint Online používa obmedzovanie na udržiavanie optimálneho výkonu a spoľahlivosti služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="57339-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="57339-108">Obmedzovanie zníži počet akcií používateľa alebo súbežných hovorov (podľa skriptu alebo kódu), aby sa zabránilo nadužívanie zdrojov.</span><span class="sxs-lookup"><span data-stu-id="57339-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="57339-109">Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="57339-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="57339-110">Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, či je aktívna údržba, ktorá sa vyskytuje na nájomníkovi, a to tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="57339-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="57339-111">Nakoniec, uistite sa, že navštívite stránku [služby zdravie](https://portal.office.com/adminportal/home#/servicehealth) skontrolovať všetky upozornenia/incidenty, ktoré môžu byť vyskytujúce.</span><span class="sxs-lookup"><span data-stu-id="57339-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

