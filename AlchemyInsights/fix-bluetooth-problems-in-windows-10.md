---
title: Riešenie problémov s Bluetooth vo Windowse 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812947"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="dea7e-102">Riešenie problémov s Bluetooth vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="dea7e-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="dea7e-103">Ak ikona Bluetooth chýba alebo bluetooth nie je možné zapnúť alebo vypnúť, pravdepodobne budete chcieť spustiť Poradcu pri riešení problémov s Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="dea7e-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="dea7e-104">[Otvorte nastavenie Riešenie problémov](ms-settings:troubleshoot), kliknite na **položku Bluetooth v** časti Vyhľadanie a riešenie **ďalších problémov** a kliknite na položku **Spustiť poradcu pri riešení problémov.**</span><span class="sxs-lookup"><span data-stu-id="dea7e-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="dea7e-105">Ak sa ikona Bluetooth nezobrazuje, ale v Správcovi zariadení sa zobrazuje Bluetooth:</span><span class="sxs-lookup"><span data-stu-id="dea7e-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="dea7e-106">V Správcovi zariadení kliknite na položku **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="dea7e-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="dea7e-107">Stlačte a podržte názov adaptéra Bluetooth (alebo naň kliknite pravým tlačidlom myši) a kliknite na položku **Odinštalovať zariadenie.**</span><span class="sxs-lookup"><span data-stu-id="dea7e-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="dea7e-108">Zatvorte zariadenie s Windowsom, počkajte niekoľko sekúnd a potom ho znova zapnite.</span><span class="sxs-lookup"><span data-stu-id="dea7e-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="dea7e-109">Windows sa pokúsi ovládač preinštalovať.</span><span class="sxs-lookup"><span data-stu-id="dea7e-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="dea7e-110">Ak ste si nedávno nainštalovali aktualizácie Windowsu 10 alebo inovované na Windows 10, možno budete chcieť vyhľadať aktualizácie ovládačov:</span><span class="sxs-lookup"><span data-stu-id="dea7e-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="dea7e-111">V Správcovi zariadení kliknite na **položku Bluetooth** a potom kliknite na názov adaptéra Bluetooth (ktorý môže obsahovať slovo "prepínač").</span><span class="sxs-lookup"><span data-stu-id="dea7e-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="dea7e-112">Stlačte a podržte adaptér Bluetooth (alebo naň kliknite pravým tlačidlom myši) a potom kliknite na položku  >  **Aktualizovať ovládač Automaticky vyhľadať aktualizovaný softvér ovládača.**</span><span class="sxs-lookup"><span data-stu-id="dea7e-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="dea7e-113">Postupujte podľa krokov a potom kliknite na tlačidlo **Zavrieť**.</span><span class="sxs-lookup"><span data-stu-id="dea7e-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="dea7e-114">Ak Windows nevie nájsť nový ovládač Bluetooth, navštívte webovú lokalitu výrobcu počítača a stiahnite si odtiaľ najnovší ovládač Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="dea7e-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="dea7e-115">Po stiahnutí kliknite na **položku** Aktualizovať ovládač Vyhľadajte v počítači softvér ovládača Vyhľadajte umiestnenie, kde sú uložené súbory  >    >   ovládačov> **OK**  >  **Ďalej** a postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="dea7e-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="dea7e-116">Po inštalácii aktualizovaného ovládača reštartujte počítač a skontrolujte, či sa tým problém s pripojením nevyrieši.</span><span class="sxs-lookup"><span data-stu-id="dea7e-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="dea7e-117">Ďalšie informácie o riešení problémov s Bluetooth nájdete v téme Riešenie problémov s [Bluetooth vo Windowse 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="dea7e-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
