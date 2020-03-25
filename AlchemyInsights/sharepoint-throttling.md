---
title: SharePoint Online obmedzovanie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931457"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="b13fe-102">SharePoint Online obmedzovanie</span><span class="sxs-lookup"><span data-stu-id="b13fe-102">SharePoint Online throttling</span></span>

<span data-ttu-id="b13fe-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="b13fe-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b13fe-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="b13fe-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b13fe-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="b13fe-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b13fe-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="b13fe-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b13fe-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="b13fe-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b13fe-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="b13fe-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b13fe-109">**SharePoint Online obmedzovanie**</span><span class="sxs-lookup"><span data-stu-id="b13fe-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="b13fe-110">SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b13fe-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b13fe-111">Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov.</span><span class="sxs-lookup"><span data-stu-id="b13fe-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="b13fe-112">Ďalšie informácie nájdete na nižšie uvedených odkazoch.</span><span class="sxs-lookup"><span data-stu-id="b13fe-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="b13fe-113">Vyhnite sa dostať škrtil alebo blokované SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b13fe-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="b13fe-114">Migrácia údajov a obmedzovanie SPO-</span><span class="sxs-lookup"><span data-stu-id="b13fe-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="b13fe-115">Rýchlosť migrácie služby SharePoint Online a OneDrive</span><span class="sxs-lookup"><span data-stu-id="b13fe-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="b13fe-116">Rukoväť SharePoint Online obmedzovanie pomocou exponenciálne späť</span><span class="sxs-lookup"><span data-stu-id="b13fe-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="b13fe-117">Plánovanie kapacity a testovanie zaťaženia SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b13fe-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

