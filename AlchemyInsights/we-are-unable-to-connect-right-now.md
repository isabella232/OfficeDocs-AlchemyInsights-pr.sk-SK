---
title: Aktivácia Problém - Sme schopní sa pripojiť práve teraz
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581890"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e75a8-102">Oprava správy aplikácie Microsoft 365 "Momentálne sa nedá pripojiť"</span><span class="sxs-lookup"><span data-stu-id="e75a8-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e75a8-103">Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúci postup:</span><span class="sxs-lookup"><span data-stu-id="e75a8-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e75a8-104">Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy, aby ste potvrdili, že neblokujú prístup na Internet k aplikáciám Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e75a8-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e75a8-105">Pozrite [si webové adresy a rozsahy adries IP od spoločnosti Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e75a8-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e75a8-106">Prejdite do ponuky **Spustiť**  >  **a**zadajte **text services.msc**.</span><span class="sxs-lookup"><span data-stu-id="e75a8-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e75a8-107">Uistite sa, že všetky nasledujúce služby sú spustené:</span><span class="sxs-lookup"><span data-stu-id="e75a8-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e75a8-108">Automatické nastavenie pripojených sieťových zariadení</span><span class="sxs-lookup"><span data-stu-id="e75a8-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e75a8-109">Služba zoznam siete</span><span class="sxs-lookup"><span data-stu-id="e75a8-109">Network List Service</span></span>
    - <span data-ttu-id="e75a8-110">Povedomie o sieťovom umiestnení</span><span class="sxs-lookup"><span data-stu-id="e75a8-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e75a8-111">Denník udalostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="e75a8-111">Windows Event Log</span></span>

<span data-ttu-id="e75a8-112">Ak nie je spustená nie ktorá z týchto služieb, skúste ju spustiť.</span><span class="sxs-lookup"><span data-stu-id="e75a8-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e75a8-113">Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s právami správcu:</span><span class="sxs-lookup"><span data-stu-id="e75a8-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e75a8-114">**Sfc / scannow SFC / scannow**</span><span class="sxs-lookup"><span data-stu-id="e75a8-114">**sfc /scannow**</span></span>

<span data-ttu-id="e75a8-115">Po dokončení tohto príkazu reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="e75a8-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e75a8-116">Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" chyba pri aktivácii balíka Office od spoločnosti Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e75a8-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>