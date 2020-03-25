---
title: SharePoint migrácie škrtenia s 503 chyby
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931673"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="f5cdf-102">SharePoint migrácie škrtenia s 503 chyby</span><span class="sxs-lookup"><span data-stu-id="f5cdf-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="f5cdf-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f5cdf-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f5cdf-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f5cdf-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f5cdf-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f5cdf-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f5cdf-109">**503 chyby pri migrácii SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="f5cdf-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="f5cdf-110">Zdá sa, že migrujete na SharePoint Online a prijímanie 503 chyby.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="f5cdf-111">Prosím, postupujte podľa nižšie uvedených krokov, aby sme vám mohli pomôcť čo najskôr.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="f5cdf-112">Kliknite na položku **kontaktovať technickú podporu**, a potom **novú servisnú požiadavku**.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="f5cdf-113">Názov a popis, zadajte **SharePoint migrácie škrtenia s 503**.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="f5cdf-114">Po tom, čo bol lístok predložený, aktualizujte ho s nasledujúcimi informáciami:</span><span class="sxs-lookup"><span data-stu-id="f5cdf-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="f5cdf-115">Koľko odišiel z migrácie (napríklad koľko TBs?).</span><span class="sxs-lookup"><span data-stu-id="f5cdf-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="f5cdf-116">Dátum začatia a ukončenia migrácie.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-116">Migration start and end date.</span></span>
    - <span data-ttu-id="f5cdf-117">Opíšte, kam migrujete svoj obsah, napríklad SharePoint Server, box, GDrive, zdieľaných súborov atď.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="f5cdf-118">Odhadnúť počet škrtenia chyby (napríklad x Throttle za hodinu?) a kedy sa škrtenia stalo.</span><span class="sxs-lookup"><span data-stu-id="f5cdf-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="f5cdf-119">Ktorý nástroj migrácie používate (napríklad SPMT alebo ShareGate).</span><span class="sxs-lookup"><span data-stu-id="f5cdf-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


