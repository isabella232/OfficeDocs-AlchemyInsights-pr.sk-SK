---
title: Riešenie problémov s aplikáciou Microsoft 365 Ľutujeme, že sa vyskytuje hlásenie s dočasným serverom
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758260"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="2c746-102">Riešenie problémov s aplikáciou Microsoft 365 Ľutujeme, že sa vyskytli problémy s dočasným serverom</span><span class="sxs-lookup"><span data-stu-id="2c746-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="2c746-103">Ak sa zobrazí toto hlásenie, vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="2c746-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2c746-104">Skontrolujte bránu firewall, antivírusový softvér a nastavenia servera proxy a potvrďte, že neblokujú prístup na internet k aplikáciám Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2c746-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2c746-105">Pozrite si tému [URL adresy a rozsahy IP adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2c746-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2c746-106">Prejdite na **položku spustiť**  >  **Spustenie**a zadajte výraz **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="2c746-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2c746-107">Uistite sa, že sú spustené tieto služby:</span><span class="sxs-lookup"><span data-stu-id="2c746-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2c746-108">Automatické nastavenie sieťových pripojení k zariadeniam</span><span class="sxs-lookup"><span data-stu-id="2c746-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2c746-109">Služba sieťového zoznamu</span><span class="sxs-lookup"><span data-stu-id="2c746-109">Network List Service</span></span>
    - <span data-ttu-id="2c746-110">Povedomie o sieťovom umiestnení</span><span class="sxs-lookup"><span data-stu-id="2c746-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2c746-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="2c746-111">Windows Event Log</span></span>

<span data-ttu-id="2c746-112">Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť.</span><span class="sxs-lookup"><span data-stu-id="2c746-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2c746-113">Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s povoleniami s právami správcu:</span><span class="sxs-lookup"><span data-stu-id="2c746-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2c746-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="2c746-114">**sfc /scannow**</span></span>

<span data-ttu-id="2c746-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="2c746-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2c746-116">Podrobné informácie nájdete v téme [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr pri aktivácii sa zobrazí chyba](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="2c746-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>