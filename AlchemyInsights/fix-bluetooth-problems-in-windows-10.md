---
title: Riešenie problémov s rozhraním Bluetooth vo Windowse 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268708"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="25810-102">Riešenie problémov s rozhraním Bluetooth vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="25810-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="25810-103">Ak chýba ikona Bluetooth alebo nie je možné zapnúť alebo vypnúť Bluetooth, možno budete chcieť spustiť Poradcu pri riešení problémov s rozhraním Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="25810-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="25810-104">[Otvorte nastavenia riešenia problémov](ms-settings:troubleshoot), kliknite na položku **Bluetooth** v časti **nájsť a opraviť ďalšie problémy**, kliknite na položku **spustiť Poradcu pri riešení problémov**.</span><span class="sxs-lookup"><span data-stu-id="25810-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="25810-105">Ak sa ikona Bluetooth nezobrazuje, ale v Správcovi zariadení sa zobrazí rozhranie Bluetooth:</span><span class="sxs-lookup"><span data-stu-id="25810-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="25810-106">V Správcovi zariadení kliknite na položku **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="25810-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="25810-107">Stlačte a podržte (alebo kliknite pravým tlačidlom myši) na názov adaptéra Bluetooth a kliknite na položku **odinštalovať zariadenie**.</span><span class="sxs-lookup"><span data-stu-id="25810-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="25810-108">Vypnite zariadenie so systémom Windows, počkajte niekoľko sekúnd a potom ho znova zapnite.</span><span class="sxs-lookup"><span data-stu-id="25810-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="25810-109">Systém Windows sa pokúsi preinštalovať ovládač.</span><span class="sxs-lookup"><span data-stu-id="25810-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="25810-110">Ak ste nedávno nainštalovali Windows 10 aktualizácie alebo inovované na Windows 10, možno budete chcieť skontrolovať aktualizácie ovládačov:</span><span class="sxs-lookup"><span data-stu-id="25810-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="25810-111">V Správcovi zariadení kliknite na položku **Bluetooth**a potom kliknite na názov adaptéra Bluetooth (ktorý môže obsahovať slovo "Radio").</span><span class="sxs-lookup"><span data-stu-id="25810-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="25810-112">Stlačte a podržte (alebo kliknite pravým tlačidlom myši) adaptér Bluetooth a potom kliknite na tlačidlo **aktualizovať Vyhľadávanie ovládačov** > **automaticky aktualizovaný softvér ovládača**.</span><span class="sxs-lookup"><span data-stu-id="25810-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="25810-113">Postupujte podľa pokynov a potom kliknite na tlačidlo **Zavrieť**.</span><span class="sxs-lookup"><span data-stu-id="25810-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="25810-114">Ak systém Windows nedokáže nájsť nový ovládač Bluetooth, navštívte webovú lokalitu výrobcu počítača a prevezmite najnovší ovládač Bluetooth odtiaľ.</span><span class="sxs-lookup"><span data-stu-id="25810-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="25810-115">Po stiahnutí, kliknite na tlačidlo **aktualizovať ovládač** > **Prehľadávať tento počítač pre softvér** > ovládača**vyhľadajte** umiestnenie, kde sú uložené súbory ovládačov > **OK** > **ďalej**a postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="25810-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="25810-116">Po inštalácii aktualizovaný ovládač, reštartujte počítač a skontrolujte, či to rieši problém s pripojením.</span><span class="sxs-lookup"><span data-stu-id="25810-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="25810-117">Pre viac informácií o tom, ako riešiť problémy s Bluetooth, prečítajte si celý článok, [opraviť Bluetooth problémy vo Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="25810-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
