---
title: Migrácia možností SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932745"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="47f88-102">Migrácia možností SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="47f88-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="47f88-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="47f88-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="47f88-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="47f88-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="47f88-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="47f88-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="47f88-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="47f88-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="47f88-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="47f88-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="47f88-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="47f88-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="47f88-109">**Možnosti migrácie**</span><span class="sxs-lookup"><span data-stu-id="47f88-109">**Migration options**</span></span>

<span data-ttu-id="47f88-110">K dispozícii sú rôzne možnosti migrácie obsahu na lokalitu SharePoint Online v závislosti od veľkosti a množstva súborov, ktoré potrebujete premiestniť, nájdete tu zoznam možností, ktoré [sa nachádzajú tu](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="47f88-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="47f88-111">Ďalšie informácie o migrácii obsahu nájdete na nižšie uvedených odkazoch.</span><span class="sxs-lookup"><span data-stu-id="47f88-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="47f88-112">Nástroj na migráciu služby SharePoint</span><span class="sxs-lookup"><span data-stu-id="47f88-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="47f88-113">Začíname pracovať s manažérom migrácie</span><span class="sxs-lookup"><span data-stu-id="47f88-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="47f88-114">Rýchlosť migrácie služby SharePoint Online a ODB</span><span class="sxs-lookup"><span data-stu-id="47f88-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="47f88-115">Vyhnite sa dostať škrtil alebo blokované SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="47f88-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="47f88-116">Nástroj na hodnotenie migrácie lokality SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="47f88-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="47f88-117">**Poznámka**: v súčasnosti SharePoint migrácia nástroj podporuje iba migrácie z lokality SharePoint 2010 a 2013.</span><span class="sxs-lookup"><span data-stu-id="47f88-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="47f88-118">Verzia 2016 alebo 2019 nie sú podporované v tomto okamihu.</span><span class="sxs-lookup"><span data-stu-id="47f88-118">Version 2016 or 2019 are not supported at this time.</span></span>
