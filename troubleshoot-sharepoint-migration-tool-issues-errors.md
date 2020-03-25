---
title: Riešenie problémov a chýb nástroja migrácia služby SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931133"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="ebcb3-102">Riešenie problémov a chýb nástroja migrácia služby SharePoint</span><span class="sxs-lookup"><span data-stu-id="ebcb3-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="ebcb3-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ebcb3-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ebcb3-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ebcb3-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ebcb3-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ebcb3-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ebcb3-109">**Bežné problémy a chyby**</span><span class="sxs-lookup"><span data-stu-id="ebcb3-109">**Common issues and errors**</span></span>

<span data-ttu-id="ebcb3-110">Pri používaní nástroja na migráciu SharePoint (SPMT) sa môžu vyskytnúť niektoré bežné problémy a chyby.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="ebcb3-111">Prosím odkaz na nižšie uvedené odkazy pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="ebcb3-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="ebcb3-112">Riešenie problémov s bežnými problémami a chybami SPMT</span><span class="sxs-lookup"><span data-stu-id="ebcb3-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="ebcb3-113">Riešenie problémov s inštaláciou SPMT</span><span class="sxs-lookup"><span data-stu-id="ebcb3-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)