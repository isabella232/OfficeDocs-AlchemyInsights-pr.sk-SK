---
title: Potrebujete pomoc s obmedzeniami odosielania e-mailov?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358356"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="e34e7-102">Potrebujete pomoc s obmedzeniami odosielania e-mailov?</span><span class="sxs-lookup"><span data-stu-id="e34e7-102">Need help with email sending limits?</span></span>

<span data-ttu-id="e34e7-103">Nižšie je **podľa-Design zasielanie limitov presadzované** v službe.</span><span class="sxs-lookup"><span data-stu-id="e34e7-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="e34e7-104">Viac informácií o týchto limitoch je zdokumentovaná [tu](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="e34e7-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="e34e7-105">Ak chcete odradiť od doručenia nevyžiadaných hromadných správ, **na všetky odchádzajúce a interné správy aplikujeme obmedzenia sadzieb príjemcov**podľa jednotlivých používateľov.</span><span class="sxs-lookup"><span data-stu-id="e34e7-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="e34e7-106">Naprieč všetkými SKUs, tento limit je **10 000 príjemcov za deň**.</span><span class="sxs-lookup"><span data-stu-id="e34e7-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="e34e7-107">Zákazníci, ktorí potrebujú posielať legitímne hromadné komerčné e-maily (napríklad zákaznícke bulletiny), by mali používať poskytovateľov tretích strán, ktorí sa špecializujú na tieto služby.</span><span class="sxs-lookup"><span data-stu-id="e34e7-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="e34e7-108">**Poznámka**: po dosiahnutí limitu počtu príjemcov sa správy nemôžu odosielať z poštovej schránky dovtedy, kým počet príjemcov odoslaných správ za posledných 24 hodín klesne pod limit.</span><span class="sxs-lookup"><span data-stu-id="e34e7-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="e34e7-109">Používateľ nebude môcť odosielať správy až do tohto bodu.</span><span class="sxs-lookup"><span data-stu-id="e34e7-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="e34e7-110">Limit rýchlosti správ **30 správ za minútu** sa aplikuje naprieč všetkými skus.</span><span class="sxs-lookup"><span data-stu-id="e34e7-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="e34e7-111">To určuje, koľko správ používateľ môže odosielať z ich konta Exchange Online v určenom období.</span><span class="sxs-lookup"><span data-stu-id="e34e7-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="e34e7-112">**Maximálny počet príjemcov povolených v poliach Komu, Kópia a Skrytá** pre jednu e-mailovú správu naprieč všetkými skus je **1000 príjemcov**.</span><span class="sxs-lookup"><span data-stu-id="e34e7-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="e34e7-113">Ak chcete prispôsobiť tento limit, choďte [sem](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="e34e7-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
