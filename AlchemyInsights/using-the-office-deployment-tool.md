---
title: Pomocou nástroja Office Deployment
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010885"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="f6cbc-102">Používanie nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="f6cbc-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f6cbc-103">Používate Office Deployment Tool (ODT) nasadiť Office 365 verzie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="f6cbc-104">Nástroj na nasadenie balíka Office (Setup. exe) je spustený z príkazového riadka a používa konfiguračný súbor XML na určenie nastavení, ktoré sa použijú pri nasadzovaní balíka Office.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="f6cbc-105">Prevezmite najnovšiu verziu nástroja na nasadenie balíka Office z [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f6cbc-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="f6cbc-106">Pomocou [nástroja na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorte súbor XML konfigurácie.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="f6cbc-107">Exportujte konfiguračný súbor a umiestnite ho lokálne na rovnaký priečinok, kde sa nachádza Setup. exe.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="f6cbc-108">**Poznámka:** Problémy s inštaláciou balíka Office sa bežne vyskytujú v dôsledku chybne nakonfigurovaných alebo chybne formátovaných konfiguračných súborov.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="f6cbc-109">Aby sa predišlo takýmto problémom, odporúčame použiť nástroj na prispôsobenie balíka Office vytvoriť konfiguračný súbor.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="f6cbc-110">Môžete tiež importovať existujúce konfiguračné súbory do nástroja na prispôsobenie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="f6cbc-111">Z príkazového riadka s právami správcu prepnite do umiestnenia, kde sa nachádza súbor Setup. exe, a spustite nástroj na nasadenie balíka Office v režime preberania a zadajte konfiguračného súboru, ktorý ste práve uložili.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="f6cbc-112">V tomto príklade konfiguračný súbor s názvom Configuration. XML:</span><span class="sxs-lookup"><span data-stu-id="f6cbc-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="f6cbc-113">Spustite nástroj Office Deployment v režime konfigurovať a zadajte konfiguračný súbor.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="f6cbc-114">**Poznámka:** Tento krok musíte spustiť z klientskeho počítača, na ktorom chcete nainštalovať balík Office a musíte mať povolenia lokálneho správcu na danom počítači.</span><span class="sxs-lookup"><span data-stu-id="f6cbc-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="f6cbc-115">Ďalšie informácie o používaní nástroja na nasadenie balíka Office pre Microsoft 365 aplikácie pre podnikové nasadenie scenáre, pozrite si [Prehľad nástroja Office Deployment](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="f6cbc-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="f6cbc-116">Ďalšie informácie o používaní nástroja na prispôsobenie balíka Office nájdete v téme [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="f6cbc-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
