---
title: Potrebujete pomoc s obmedzeniami odosielania e-mailov?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836294"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="2dad0-102">Potrebujete pomoc s obmedzeniami odosielania e-mailov?</span><span class="sxs-lookup"><span data-stu-id="2dad0-102">Need help with email sending limits?</span></span>

<span data-ttu-id="2dad0-103">Nižšie sú uvedené **limity odosielania na základe návrhu,** ktoré sa vynútejú v službe.</span><span class="sxs-lookup"><span data-stu-id="2dad0-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="2dad0-104">Ďalšie informácie o týchto obmedzeniach nájdete v [dokumente](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="2dad0-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="2dad0-105">Na to, aby sme neodporúčali doručovanie nevyžiadaných hromadných správ, na všetky odchádzajúce a interné správy používame limity týkajúce sa frekvencie príjemcov **podľa používateľa.**</span><span class="sxs-lookup"><span data-stu-id="2dad0-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="2dad0-106">Vo všetkých SKU je tento limit **10 000 príjemcov za deň.**</span><span class="sxs-lookup"><span data-stu-id="2dad0-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="2dad0-107">Zákazníci, ktorí potrebujú odosielať legitímne hromadné komerčné e-maily (napríklad zákaznícke bulletiny), by mali používať poskytovateľov tretích strán, ktorí sa v týchto službách špecializovaní na tieto služby.</span><span class="sxs-lookup"><span data-stu-id="2dad0-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="2dad0-108">**Poznámka:** Po dosiahol sa limit frekvencie príjemcov, správy z poštovej schránky nie je možné odosielať, kým počet príjemcov, ktorí boli odoslaní v priebehu posledných 24 hodín, nedosune limit.</span><span class="sxs-lookup"><span data-stu-id="2dad0-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="2dad0-109">Dovtedy používateľ nebude môcť odosielať správy.</span><span class="sxs-lookup"><span data-stu-id="2dad0-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="2dad0-110">Limit frekvencie správ **pre 30 správ za minútu sa** používa vo všetkých SKU.</span><span class="sxs-lookup"><span data-stu-id="2dad0-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="2dad0-111">Tým sa určuje, koľko správ môže používateľ odoslať zo svojho konta Exchange Online v rámci zadaného obdobia.</span><span class="sxs-lookup"><span data-stu-id="2dad0-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="2dad0-112">Maximálny povolený počet príjemcov v poliach **Komu,** Kópia a Skrytá pre jednu e-mailovú správu v rámci všetkých SKU je **1 000 príjemcov.**</span><span class="sxs-lookup"><span data-stu-id="2dad0-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="2dad0-113">Ak chcete tento limit prispôsobiť, prejdite [sem.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="2dad0-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
