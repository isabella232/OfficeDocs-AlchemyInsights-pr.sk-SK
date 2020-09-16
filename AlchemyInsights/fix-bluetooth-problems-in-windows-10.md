---
title: Riešenie problémov s technológiou Bluetooth vo Windowse 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730174"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="3e872-102">Riešenie problémov s technológiou Bluetooth vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="3e872-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="3e872-103">Ak chýba ikona Bluetooth alebo nie je možné zapnúť alebo vypnúť Bluetooth, možno budete chcieť spustiť Poradcu pri riešení problémov s technológiou Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="3e872-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="3e872-104">[Otvorte nastavenia riešenia problémov](ms-settings:troubleshoot), kliknite na položku **Bluetooth** v časti **Vyhľadať a opraviť ďalšie problémy**, kliknite na položku **spustiť Poradcu pri riešení problémov**.</span><span class="sxs-lookup"><span data-stu-id="3e872-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="3e872-105">Ak sa ikona Bluetooth nezobrazuje, v Správcovi zariadení sa však zobrazí Bluetooth:</span><span class="sxs-lookup"><span data-stu-id="3e872-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="3e872-106">V Správcovi zariadení kliknite na položku **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="3e872-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="3e872-107">Stlačte a podržte názov adaptéra Bluetooth (alebo naň kliknite pravým tlačidlom myši) a kliknite na položku **odinštalovať zariadenie**.</span><span class="sxs-lookup"><span data-stu-id="3e872-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="3e872-108">Vypnite zariadenie s Windowsom, počkajte niekoľko sekúnd a potom ho znova zapnite.</span><span class="sxs-lookup"><span data-stu-id="3e872-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="3e872-109">Systém Windows sa pokúsi preinštalovať ovládač.</span><span class="sxs-lookup"><span data-stu-id="3e872-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="3e872-110">Ak ste nedávno nainštalovali aktualizácie Windowsu 10 alebo inovovali na Windows 10, možno budete chcieť vyhľadať aktualizácie ovládačov:</span><span class="sxs-lookup"><span data-stu-id="3e872-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="3e872-111">V Správcovi zariadení kliknite na položku **Bluetooth**a potom kliknite na názov adaptéra Bluetooth (ktorý môže obsahovať slovo Radio).</span><span class="sxs-lookup"><span data-stu-id="3e872-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="3e872-112">Stlačte a podržte adaptér Bluetooth (alebo naň kliknite pravým tlačidlom myši) a potom kliknite na položku **aktualizovať ovládač**  >  **automaticky vyhľadávať aktualizovaný softvér ovládača**.</span><span class="sxs-lookup"><span data-stu-id="3e872-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="3e872-113">Postupujte podľa pokynov a potom kliknite na položku **zatvorenie**.</span><span class="sxs-lookup"><span data-stu-id="3e872-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="3e872-114">Ak Windows nedokáže nájsť nový ovládač Bluetooth, navštívte webovú lokalitu výrobcu počítača a Stiahnite si z neho najnovší ovládač Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="3e872-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="3e872-115">Po stiahnutí kliknite na položku **aktualizovať ovládač**  >  **vyhľadajte v počítači ovládač softvéru**  >  **vyhľadajte** umiestnenie, v ktorom sú súbory ovládača uložené > **tlačidlo OK**  >  **ďalej**a postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="3e872-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="3e872-116">Po inštalácii aktualizovaného ovládača reštartujte počítač a skontrolujte, či je problém s pripojením vyriešený.</span><span class="sxs-lookup"><span data-stu-id="3e872-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="3e872-117">Ďalšie informácie o riešení problémov s technológiou Bluetooth nájdete v celom článku [Riešenie problémov s technológiou Bluetooth vo Windowse 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="3e872-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
