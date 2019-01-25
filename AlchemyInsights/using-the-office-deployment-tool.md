---
title: Pomocou nástroja nasadenia Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488575"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="954de-102">Pomocou Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="954de-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="954de-p101">Nasadiť Office 365 verzie balíka Office pomocou Office Deployment Tool (ODT). Office Deployment Tool (setup.exe) je spustiť z príkazového riadka a používa konfiguračný XML súbor zistiť, aké nastavenia použiť pri nasadzovaní balíka Office.</span><span class="sxs-lookup"><span data-stu-id="954de-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="954de-105">Stiahnite si najnovšiu verziu nástroja nasadenia Office z [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="954de-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="954de-p102">Použite [Nástroj na prispôsobenie balíka Office (OCT)](https://config.office.com) vyberte predvoľby nasadenia a vytvorenie konfiguračného XML súboru. Export konfiguračný súbor a umiestnite ho lokálne v rovnakom priečinku kde býva setup.exe.</span><span class="sxs-lookup"><span data-stu-id="954de-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="954de-p103">**Poznámka:** Inštaláciu balíka Office bežne vyskytnúť problémy vzhľadom na zle alebo malformatted konfiguračné súbory. Aby sa predišlo také problémy, odporúčame, že používate nástroj na prispôsobenie balíka Office vytvoriť konfiguračný súbor. Môžete tiež importovať existujúce konfiguračné súbory do nástroj na prispôsobenie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="954de-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="954de-p104">Z námer kontrolovať vrtký, prepnite do polohy bydliska setup.exe a spustite nástroj na nasadenie balíka Office v režime stiahnutie a určite konfiguračný súbor ste práve uložili. V tomto príklade, konfiguračný súbor sa nazýva Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="954de-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="954de-113">Spustenie nástroja nasadenia Office v Konfigurácia režimu a zadajte konfiguračný súbor.</span><span class="sxs-lookup"><span data-stu-id="954de-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="954de-114">**Poznámka:** Tento krok musíte spustiť z klientskeho počítača, na ktorom chcete nainštalovať balík Office a musíte mať povolenia lokálneho správcu na tomto počítači.</span><span class="sxs-lookup"><span data-stu-id="954de-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="954de-p105">Ďalšie informácie o používaní nástroja nasadenia Office pre Office 365 ProPlus scenáre nasadenia, pozrite si [Prehľad nástroja nasadenia Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Pre viac informácií o tom, ako používať nástroj na prispôsobenie balíka Office, nájdete v časti [Prehľad nástroja na prispôsobenie balíka Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="954de-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

