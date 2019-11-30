---
title: Aktivácia problém-sme schopní sa pripojiť práve teraz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628257"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="6afb2-102">Oprava aplikácie balíka Office "sme schopní pripojiť práve teraz" správa</span><span class="sxs-lookup"><span data-stu-id="6afb2-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="6afb2-103">Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="6afb2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6afb2-104">Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office.</span><span class="sxs-lookup"><span data-stu-id="6afb2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="6afb2-105">Pozrite si [Office 365 adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6afb2-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6afb2-106">Prejdite na **Štart** > **Spustiť**, a potom zadajte **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="6afb2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6afb2-107">Uistite sa, že sú spustené nasledujúce služby:</span><span class="sxs-lookup"><span data-stu-id="6afb2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6afb2-108">Automatické nastavenie zariadení pripojených k sieti</span><span class="sxs-lookup"><span data-stu-id="6afb2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6afb2-109">Služba sieťového zoznamu</span><span class="sxs-lookup"><span data-stu-id="6afb2-109">Network List Service</span></span>
    - <span data-ttu-id="6afb2-110">Povedomie o umiestnení v sieti</span><span class="sxs-lookup"><span data-stu-id="6afb2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6afb2-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="6afb2-111">Windows Event Log</span></span>

<span data-ttu-id="6afb2-112">Ak jedna z týchto služieb nie je spustená, pokúste sa ho spustiť.</span><span class="sxs-lookup"><span data-stu-id="6afb2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6afb2-113">Ak máte problém so spustením služby, spustite nasledovný príkaz otvorením príkazového riadka so zvýšenými povoleniami:</span><span class="sxs-lookup"><span data-stu-id="6afb2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6afb2-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="6afb2-114">**sfc /scannow**</span></span>

<span data-ttu-id="6afb2-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="6afb2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6afb2-116">Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr "chyba pri aktivácii balíka Office z balíka Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="6afb2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>