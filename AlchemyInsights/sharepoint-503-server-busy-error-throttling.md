---
title: SharePoint Online obmedzovanie
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048631"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="e6bfe-102">SharePoint Online obmedzovanie</span><span class="sxs-lookup"><span data-stu-id="e6bfe-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="e6bfe-103">Používatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="e6bfe-104">Táto chyba môže byť spôsobená škrtenia v službe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="e6bfe-105">SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="e6bfe-106">Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="e6bfe-107">Ak sa vám škrtil, 99% času je to preto, že vlastný kód.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="e6bfe-108">Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="e6bfe-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="e6bfe-109">Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, či je aktívna údržba, ktorá sa vyskytuje na nájomníkovi, a to tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="e6bfe-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="e6bfe-110">Nakoniec, uistite sa, že navštívite stránku [služby zdravie](https://portal.office.com/adminportal/home#/servicehealth) skontrolovať všetky upozornenia/incidenty, ktoré môžu byť vyskytujúce.</span><span class="sxs-lookup"><span data-stu-id="e6bfe-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

