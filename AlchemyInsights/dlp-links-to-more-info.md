---
title: Viac informácií o problémoch s DLP
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932709"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="e16f2-102">Informácie o problémoch s DLP</span><span class="sxs-lookup"><span data-stu-id="e16f2-102">Information about DLP issues</span></span>

<span data-ttu-id="e16f2-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="e16f2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e16f2-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="e16f2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e16f2-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="e16f2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e16f2-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="e16f2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e16f2-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="e16f2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e16f2-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="e16f2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e16f2-109">**Informácie o politike DLP**</span><span class="sxs-lookup"><span data-stu-id="e16f2-109">**Information on DLP policy**</span></span>

<span data-ttu-id="e16f2-110">S politikou DLP môžete identifikovať, monitorovať a automaticky chrániť citlivé informácie v rámci balíka Office 365.</span><span class="sxs-lookup"><span data-stu-id="e16f2-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="e16f2-111">Ďalšie informácie nájdete na týchto odkazoch:</span><span class="sxs-lookup"><span data-stu-id="e16f2-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="e16f2-112">Prehľad prevencie straty údajov</span><span class="sxs-lookup"><span data-stu-id="e16f2-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="e16f2-113">Aké typy citlivých informácií vyzerajú</span><span class="sxs-lookup"><span data-stu-id="e16f2-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="e16f2-114">Vytvorenie vlastného typu citlivých informácií</span><span class="sxs-lookup"><span data-stu-id="e16f2-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="e16f2-115">Odoslať e-mailové upozornenia a Zobraziť tipy politiky</span><span class="sxs-lookup"><span data-stu-id="e16f2-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="e16f2-116">Chráňte súbory SharePoint Online s menovkami uchovávania údajov a DLP</span><span class="sxs-lookup"><span data-stu-id="e16f2-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="e16f2-117">DLP a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="e16f2-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="e16f2-118">Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **typ testu** podľa **klasifikácie** > **citlivých typov**informácií.</span><span class="sxs-lookup"><span data-stu-id="e16f2-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e16f2-119">Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="e16f2-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>