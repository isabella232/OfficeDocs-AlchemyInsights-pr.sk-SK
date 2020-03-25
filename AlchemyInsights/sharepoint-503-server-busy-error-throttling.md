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
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931241"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="6acb7-102">SharePoint Online obmedzovanie</span><span class="sxs-lookup"><span data-stu-id="6acb7-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="6acb7-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="6acb7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6acb7-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="6acb7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6acb7-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="6acb7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6acb7-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="6acb7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6acb7-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="6acb7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6acb7-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="6acb7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6acb7-109">**503 server je zaneprázdnený chyba**</span><span class="sxs-lookup"><span data-stu-id="6acb7-109">**503 server is busy error**</span></span>

<span data-ttu-id="6acb7-110">Používatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6acb7-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="6acb7-111">Táto chyba môže byť spôsobená škrtenia v službe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6acb7-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6acb7-112">SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6acb7-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6acb7-113">Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="6acb7-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="6acb7-114">Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6acb7-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="6acb7-115">Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, či je aktívna údržba, ktorá sa vyskytuje na nájomníkovi, a to tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="6acb7-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="6acb7-116">Nakoniec, uistite sa, že navštívite stránku [služby zdravie](https://portal.office.com/adminportal/home#/servicehealth) skontrolovať všetky upozornenia/incidenty, ktoré môžu byť vyskytujúce.</span><span class="sxs-lookup"><span data-stu-id="6acb7-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

