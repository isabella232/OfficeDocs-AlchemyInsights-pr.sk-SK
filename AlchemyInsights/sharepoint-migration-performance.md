---
title: Výkon migrácie SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932403"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="3e46b-102">Výkon migrácie SharePoint</span><span class="sxs-lookup"><span data-stu-id="3e46b-102">SharePoint migration performance</span></span>

<span data-ttu-id="3e46b-103">**Dôležité**: Mnoho zákazníkov SharePointu Online a OneDrivu spúšťa dôležité podnikové aplikácie s pomocou služby, ktorá beží na pozadí.</span><span class="sxs-lookup"><span data-stu-id="3e46b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3e46b-104">Patrí sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="3e46b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3e46b-105">V tomto neobvyklom období podnikáme kroky, aby boli služby SharePoint Online a OneDrive i naďalej vysoko dostupné a spoľahlivé pre vašich používateľov, ktorí sa v súčasnosti viac ako zvyčajne spoliehajú na túto službu pri práci na diaľku.</span><span class="sxs-lookup"><span data-stu-id="3e46b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3e46b-106">Na dosiahnutie tohto cieľa sme implementovali prísnejšie obmedzenia aplikácií na pozadí (migrácia, DLP a riešenia zálohovania) počas denných hodín pracovných dní.</span><span class="sxs-lookup"><span data-stu-id="3e46b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3e46b-107">Mali by ste očakávať, že tieto aplikácie dosiahnu v týchto časoch veľmi obmedzenú priepustnosť.</span><span class="sxs-lookup"><span data-stu-id="3e46b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3e46b-108">Počas večerných a víkendových hodín pre príslušnú oblasť však bude služba pripravená na spracovanie významne vyššieho objemu požiadaviek z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="3e46b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3e46b-109">**Výkon migrácie**</span><span class="sxs-lookup"><span data-stu-id="3e46b-109">**Migration performance**</span></span>

<span data-ttu-id="3e46b-110">Výkon migrácie môže byť ovplyvnený sieťovou infraštruktúrou, veľkosťou súborov, časom migrácie a obmedzovaním.</span><span class="sxs-lookup"><span data-stu-id="3e46b-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="3e46b-111">Porozumenie týmto faktorom vám pomôže pri plánovaní a maximalizácii efektivity migrácie.</span><span class="sxs-lookup"><span data-stu-id="3e46b-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="3e46b-112">Ďalšie informácie nájdete na prepojeniach nižšie.</span><span class="sxs-lookup"><span data-stu-id="3e46b-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="3e46b-113">Rýchlosť služby SharePoint Online a migrácie ODB</span><span class="sxs-lookup"><span data-stu-id="3e46b-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="3e46b-114">Ako sa vyhnúť obmedzeniam toku údajov alebo zablokovaniu v SharePointe Online</span><span class="sxs-lookup"><span data-stu-id="3e46b-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="3e46b-115">Stiahnutie a inštalácia nástroja na migráciu SharePointu</span><span class="sxs-lookup"><span data-stu-id="3e46b-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
