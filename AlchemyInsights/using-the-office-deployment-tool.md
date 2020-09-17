---
title: Používanie nástroja na nasadenie balíka Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794926"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="87858-102">Použitie nástroja na nasadenie balíka Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="87858-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="87858-103">Pomocou nástroja na nasadenie balíka Office (ODT) môžete nasadiť verzie balíka Office 365.</span><span class="sxs-lookup"><span data-stu-id="87858-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="87858-104">Nástroj na nasadenie balíka Office (setup.exe) sa spustí z príkazového riadkov a použije súbor konfigurácie XML na určenie nastavení, ktoré sa majú použiť pri nasadení balíka Office.</span><span class="sxs-lookup"><span data-stu-id="87858-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="87858-105">Stiahnite si najnovšiu verziu nástroja na nasadenie balíka Office z [Centra sťahovania](https://go.microsoft.com/fwlink/p/?LinkID=626065)softvéru.</span><span class="sxs-lookup"><span data-stu-id="87858-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="87858-106">Pomocou [nástroja na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorte súbor XML konfigurácie.</span><span class="sxs-lookup"><span data-stu-id="87858-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="87858-107">Exportujte konfiguračný súbor a umiestnite ho lokálne do rovnakého priečinka, v ktorom sa nachádza setup.exe.</span><span class="sxs-lookup"><span data-stu-id="87858-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="87858-108">**Poznámka:** Problémy s inštaláciou balíka Office sa bežne vyskytujú v dôsledku nesprávne konfigurovaných alebo malformatted konfiguračných súborov.</span><span class="sxs-lookup"><span data-stu-id="87858-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="87858-109">Ak sa chcete vyhnúť takýmto problémom, odporúčame, aby ste na vytvorenie konfiguračného súboru použili nástroj na prispôsobenie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="87858-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="87858-110">Existujúce konfiguračné súbory môžete importovať aj do nástroja na prispôsobenie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="87858-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="87858-111">V príkazovom riadku s právami správcu prejdite na miesto, kde sa setup.exe nachádza, a spustite nástroj na nasadenie balíka Office v režime sťahovania a zadajte konfiguračný súbor, ktorý ste práve uložili.</span><span class="sxs-lookup"><span data-stu-id="87858-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="87858-112">V tomto príklade sa konfiguračný súbor nazýva Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="87858-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="87858-113">4. Spustite nástroj na nasadenie balíka Office v režime konfigurácie a zadajte konfiguračný súbor.</span><span class="sxs-lookup"><span data-stu-id="87858-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="87858-114">**Poznámka:** Tento krok musíte spustiť z klientskeho počítača, v ktorom chcete nainštalovať balík Office, a musíte mať v danom počítači povolenia lokálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="87858-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="87858-115">Ďalšie informácie o používaní nástroja na nasadenie balíka Office pre aplikácie Microsoft 365 pre scenáre podnikového nasadenia nájdete v téme [Prehľad nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="87858-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="87858-116">Ďalšie informácie o používaní nástroja na prispôsobenie balíka Office nájdete v téme [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="87858-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
