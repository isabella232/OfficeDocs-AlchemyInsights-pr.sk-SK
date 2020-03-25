---
title: Problémy pri migrácii údajov SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931709"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="e70ff-102">Problémy pri migrácii údajov SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e70ff-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="e70ff-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="e70ff-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e70ff-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="e70ff-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e70ff-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="e70ff-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e70ff-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="e70ff-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e70ff-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="e70ff-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e70ff-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="e70ff-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e70ff-109">**Migrácia cez 100TB údajov**</span><span class="sxs-lookup"><span data-stu-id="e70ff-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="e70ff-110">Zdá sa, že migrujete viac ako 100TB údajov na SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e70ff-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="e70ff-111">Prosím, postupujte podľa nižšie uvedených krokov, aby sme vám mohli pomôcť čo najskôr.</span><span class="sxs-lookup"><span data-stu-id="e70ff-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="e70ff-112">Vyberte **novú servisnú požiadavku**a potom **novú servisnú požiadavku**.</span><span class="sxs-lookup"><span data-stu-id="e70ff-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="e70ff-113">Ponechať názov a popis ako **migrácia služby SharePoint cez 100TB**.</span><span class="sxs-lookup"><span data-stu-id="e70ff-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="e70ff-114">Po tom, čo bol lístok predložený, aktualizujte ho s nasledujúcimi informáciami:</span><span class="sxs-lookup"><span data-stu-id="e70ff-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="e70ff-115">Odhadovaná veľkosť migrácie.</span><span class="sxs-lookup"><span data-stu-id="e70ff-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="e70ff-116">Odhad, Kedy by ste chceli začať a dokončiť migráciu.</span><span class="sxs-lookup"><span data-stu-id="e70ff-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="e70ff-117">Opíšte, kam migrujete svoj obsah, napríklad SharePoint Server, box, GDrive, zdieľaných súborov atď.</span><span class="sxs-lookup"><span data-stu-id="e70ff-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

