---
title: Politika zdieľania kalendára 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684245"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="1dca3-102">Chyba politiky pri zdieľaní kalendára</span><span class="sxs-lookup"><span data-stu-id="1dca3-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="1dca3-103">Vykonajte niektorý z týchto krokov, ktoré zodpovedajú vašej situácii:</span><span class="sxs-lookup"><span data-stu-id="1dca3-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="1dca3-104">Pripojte sa k službe Exchange Online pomocou vzdialeného prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1dca3-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="1dca3-105">Ďalšie informácie nájdete v téme [pripojenie k službe Exchange Online pomocou vzdialeného prostredia PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1dca3-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="1dca3-106">Na lokálnom serveri Otvorte prostredie Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="1dca3-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="1dca3-107">Určenie politiky zdieľania, ktorá je priradená používateľovi.</span><span class="sxs-lookup"><span data-stu-id="1dca3-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="1dca3-108">Ak to chcete urobiť, spustite nasledujúci príkaz a zaznamenajte si politiku, ktorá sa vrátila:</span><span class="sxs-lookup"><span data-stu-id="1dca3-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="1dca3-109">Aktualizujte politiku zdieľania pre používateľa.</span><span class="sxs-lookup"><span data-stu-id="1dca3-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="1dca3-110">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="1dca3-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="1dca3-111">Otvorte Centrum spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dca3-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="1dca3-112">Kliknite na položku **organizácia**a potom dvakrát kliknite na politiku, ktorá je priradená používateľovi v rámci **individuálneho zdieľania**.</span><span class="sxs-lookup"><span data-stu-id="1dca3-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="1dca3-113">Toto je politika, ktorá bola vrátená v kroku 2.</span><span class="sxs-lookup"><span data-stu-id="1dca3-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="1dca3-114">Na stránke pravidlo zdieľania vyberte úroveň zdieľania kalendára, ktorú chcete povoliť v časti **určenie informácií, ktoré chcete zdieľať**. kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="1dca3-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="1dca3-115">Ďalšie informácie nájdete v téme: [politika nepovoľuje udeliť povolenia na úrovni jednej alebo viacerým príjemcom pri pokuse o zdieľanie kalendára](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="1dca3-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
