---
title: Obmedzovanie SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761273"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="67e1a-102">Obmedzovanie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="67e1a-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="67e1a-103">Užívatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse prejsť na lokalitách SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="67e1a-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="67e1a-104">Táto chyba môže spôsobené škrtenia v rámci služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="67e1a-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="67e1a-105">SharePoint Online používa škrtenia na zachovanie optimálneho výkonu a spoľahlivosti služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="67e1a-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="67e1a-106">Obmedzovanie limity počtu akcií používateľa alebo súbežných volania (podľa skript alebo kód) aby sa predišlo nadužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="67e1a-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="67e1a-107">Ak ste dostať škrtil, 99% času je to kvôli vlastný kód.</span><span class="sxs-lookup"><span data-stu-id="67e1a-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="67e1a-108">Ďalšie informácie o rdoušení pozri, [Vyhnite sa stále obmedzené alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="67e1a-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="67e1a-109">Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, ak je aktívna údržba vyskytujúce sa na nájomcu prechodom do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="67e1a-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="67e1a-110">Nakoniec, zabezpečiť navštívite stránku [Stav služby](https://portal.office.com/adminportal/home#/servicehealth) zistiť akékoľvek upozornenia/incidentov, ktoré sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="67e1a-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

