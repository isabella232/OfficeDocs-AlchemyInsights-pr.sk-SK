---
title: Oprava aplikácií balíka Office Ospravedlňujeme sa, máme dočasný server problémy správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764132"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="4a8ac-102">Upevnenie aplikácie balíka Office "Ospravedlňujeme sa, máme dočasný server problémy" správa</span><span class="sxs-lookup"><span data-stu-id="4a8ac-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="4a8ac-103">Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="4a8ac-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4a8ac-104">Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="4a8ac-105">Pozrite si [adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="4a8ac-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4a8ac-106">Prejdite na **Štart** > **Spustiť**, a potom zadajte **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4a8ac-107">Uistite sa, že sú spustené nasledujúce služby:</span><span class="sxs-lookup"><span data-stu-id="4a8ac-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4a8ac-108">Automatické nastavenie zariadení pripojených k sieti</span><span class="sxs-lookup"><span data-stu-id="4a8ac-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4a8ac-109">Služba sieťového zoznamu</span><span class="sxs-lookup"><span data-stu-id="4a8ac-109">Network List Service</span></span>
    - <span data-ttu-id="4a8ac-110">Povedomie o umiestnení v sieti</span><span class="sxs-lookup"><span data-stu-id="4a8ac-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4a8ac-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="4a8ac-111">Windows Event Log</span></span>

<span data-ttu-id="4a8ac-112">Ak jedna z týchto služieb nie je spustená, pokúste sa ho spustiť.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4a8ac-113">Ak máte problém so spustením služby, spustite nasledovný príkaz otvorením príkazového riadka so zvýšenými povoleniami:</span><span class="sxs-lookup"><span data-stu-id="4a8ac-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4a8ac-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-114">**sfc /scannow**</span></span>

<span data-ttu-id="4a8ac-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4a8ac-116">Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Prosím, skúste to znova neskôr "chyba pri aktivácii](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="4a8ac-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>