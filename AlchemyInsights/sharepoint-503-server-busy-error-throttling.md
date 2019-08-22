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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559856"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="37788-102">Obmedzovanie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="37788-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="37788-103">Užívatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse prejsť na lokalitách SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37788-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="37788-104">Táto chyba môže spôsobené škrtenia v rámci služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="37788-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="37788-105">SharePoint Online používa škrtenia na zachovanie optimálneho výkonu a spoľahlivosti služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="37788-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="37788-106">Obmedzovanie limity počtu akcií používateľa alebo súbežných volania (podľa skript alebo kód) aby sa predišlo nadužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="37788-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="37788-107">Ak ste dostať škrtil, 99% času je to kvôli vlastný kód.</span><span class="sxs-lookup"><span data-stu-id="37788-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="37788-108">Ďalšie informácie o rdoušení pozri, [Vyhnite sa stále obmedzené alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="37788-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="37788-109">Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, ak je aktívna údržba vyskytujúce sa na nájomcu prechodom do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="37788-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="37788-110">Nakoniec, zabezpečiť navštívite stránku [Stav služby](https://portal.office.com/adminportal/home#/servicehealth) zistiť akékoľvek upozornenia/incidentov, ktoré sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="37788-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

