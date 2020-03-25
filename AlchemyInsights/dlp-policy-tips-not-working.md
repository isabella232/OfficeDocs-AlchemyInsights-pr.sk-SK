---
title: DLP politika tipy nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932601"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="44edd-102">Problémy s tipmi politiky DLP</span><span class="sxs-lookup"><span data-stu-id="44edd-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="44edd-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="44edd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="44edd-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="44edd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="44edd-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="44edd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="44edd-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="44edd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="44edd-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="44edd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="44edd-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="44edd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="44edd-109">**Tipy pre politiku DLP**</span><span class="sxs-lookup"><span data-stu-id="44edd-109">**DLP policy tips**</span></span>

<span data-ttu-id="44edd-110">Pri používaní **politík DLP**môžu byť používatelia upozornení na porušenie pravidiel pomocou **tipov politiky**.</span><span class="sxs-lookup"><span data-stu-id="44edd-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="44edd-111">Správcovia môžu nakonfigurovať politiky tipy na zobrazenie pri testovaní ich DLP politiky alebo keď politika je v režime úplného výkonu.</span><span class="sxs-lookup"><span data-stu-id="44edd-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="44edd-112">Ak chcete konfigurovať tipy politiky v politike DLP v centre zabezpečenia a súladu v úplnom režime výkonu, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="44edd-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="44edd-113">Uistite sa, že politiky tipy boli **povolené** na DLP pravidlo pomocou krokov [tu](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="44edd-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="44edd-114">Uistite sa, že váš **obsah zodpovedá** tomu, čo je **potrebné** na spustenie pravidla načrtnutého v tomto článku [tu](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="44edd-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="44edd-115">Politika tipy Zobraziť v OWA a Outlook.</span><span class="sxs-lookup"><span data-stu-id="44edd-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="44edd-116">Avšak, pri používaní **programu Outlook 2013 alebo novší**, politiky tipy sú zobrazené len za určitých podmienok.</span><span class="sxs-lookup"><span data-stu-id="44edd-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="44edd-117">Tieto podmienky sú uvedené tu: [podporované podmienky pre program Outlook 2013 alebo novší pre zobrazenie politiky tipy](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="44edd-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="44edd-118">Ďalšie informácie o tipy pre politiku DLP nájdete v téme: [Zobraziť tipy politiky pre politiky DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="44edd-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  