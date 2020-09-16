---
title: Problém s aktiváciou – momentálne sa nemôžeme pripojiť
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725998"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b9ee3-102">Riešenie problémov s aplikáciou Microsoft 365 sa momentálne nedá pripojiť</span><span class="sxs-lookup"><span data-stu-id="b9ee3-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b9ee3-103">Ak sa zobrazí toto hlásenie, vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="b9ee3-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b9ee3-104">Skontrolujte bránu firewall, antivírusový softvér a nastavenia servera proxy a potvrďte, že neblokujú prístup na internet k aplikáciám Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b9ee3-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b9ee3-105">Pozrite si tému [URL adresy a rozsahy IP adries spoločnosti Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b9ee3-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b9ee3-106">Prejdite na **položku spustiť**  >  **Spustenie**a zadajte výraz **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="b9ee3-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b9ee3-107">Uistite sa, že sú spustené tieto služby:</span><span class="sxs-lookup"><span data-stu-id="b9ee3-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b9ee3-108">Automatické nastavenie sieťových pripojení k zariadeniam</span><span class="sxs-lookup"><span data-stu-id="b9ee3-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b9ee3-109">Služba sieťového zoznamu</span><span class="sxs-lookup"><span data-stu-id="b9ee3-109">Network List Service</span></span>
    - <span data-ttu-id="b9ee3-110">Povedomie o sieťovom umiestnení</span><span class="sxs-lookup"><span data-stu-id="b9ee3-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b9ee3-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="b9ee3-111">Windows Event Log</span></span>

<span data-ttu-id="b9ee3-112">Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť.</span><span class="sxs-lookup"><span data-stu-id="b9ee3-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b9ee3-113">Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s povoleniami s právami správcu:</span><span class="sxs-lookup"><span data-stu-id="b9ee3-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b9ee3-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="b9ee3-114">**sfc /scannow**</span></span>

<span data-ttu-id="b9ee3-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="b9ee3-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b9ee3-116">Podrobné informácie nájdete v téme [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr "chyba pri aktivácii balíka Office z Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b9ee3-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>