---
title: Problém s aktiváciou – nepodarilo sa nám pripojiť
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806457"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="dc323-102">Oprava správy o aplikáciách služby Microsoft 365 "Nepodarilo sa pripojiť"</span><span class="sxs-lookup"><span data-stu-id="dc323-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="dc323-103">Ak sa zobrazí toto hlásenie, skúste toto:</span><span class="sxs-lookup"><span data-stu-id="dc323-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="dc323-104">Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k aplikáciám služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dc323-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="dc323-105">Pozrite [si časť URL adresy a rozsahy IP adries od spoločnosti Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="dc323-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="dc323-106">Prejdite do **ponuky**  >  **Spustiť spustenie** a zadajte reťazec **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="dc323-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="dc323-107">Skontrolujte, či sú spustené všetky tieto služby:</span><span class="sxs-lookup"><span data-stu-id="dc323-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="dc323-108">Automatické nastavenie zariadení pripojených k sieti</span><span class="sxs-lookup"><span data-stu-id="dc323-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="dc323-109">Služba so zoznamom sietí</span><span class="sxs-lookup"><span data-stu-id="dc323-109">Network List Service</span></span>
    - <span data-ttu-id="dc323-110">Informovanosť o sieťovom umiestnení</span><span class="sxs-lookup"><span data-stu-id="dc323-110">Network Location Awareness</span></span>
    - <span data-ttu-id="dc323-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="dc323-111">Windows Event Log</span></span>

<span data-ttu-id="dc323-112">Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť.</span><span class="sxs-lookup"><span data-stu-id="dc323-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="dc323-113">Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s zvýšenými povoleniami:</span><span class="sxs-lookup"><span data-stu-id="dc323-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="dc323-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="dc323-114">**sfc /scannow**</span></span>

<span data-ttu-id="dc323-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="dc323-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="dc323-116">Podrobné informácie nájdete v časti [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" pri aktivácii balíka Office zo služby Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="dc323-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>