---
title: Ikona napájania alebo batérie chýba vo Windowse 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790563"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="9da8c-102">Ikona napájania alebo batérie chýba vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="9da8c-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="9da8c-103">Ak vaše zariadenie s Windowsom 10 obsahuje batériu (napríklad notebook alebo tablet alebo počítač pripojený cez USB k záložnému zdroju UPS), na paneli úloh v blízkosti hodín sa zvyčajne zobrazuje ikona napájania alebo batérie, napríklad:</span><span class="sxs-lookup"><span data-stu-id="9da8c-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona batérie](media/battery-icon.png)

<span data-ttu-id="9da8c-105">Ak sa táto ikona nezobrazuje, môže byť skrytá:</span><span class="sxs-lookup"><span data-stu-id="9da8c-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="9da8c-106">Prejdite na položky **[Nastavenia > Prispôsobenie > Panel úloh](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="9da8c-107">V časti Oblasť oznámení kliknite na položku **Vyberte ikony, ktoré sa budú zobrazovať na paneli úloh**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="9da8c-108">Potom v zozname vyhľadajte položku **Napájanie** a prepnite jej nastavenie na možnosť **Zapnuté**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Zobrazenie ikony napájania na paneli úloh](media/power-icon-on.png)

<span data-ttu-id="9da8c-110">**Riešenie problémov**</span><span class="sxs-lookup"><span data-stu-id="9da8c-110">**Troubleshooting**</span></span>

<span data-ttu-id="9da8c-111">Ak ste postupovali podľa uvedených pokynov a prepínač **Napájanie** je sivý alebo sa nezobrazuje, do vyhľadávacieho poľa na paneli úloh napíšte výraz **správca zariadení** a potom v zozname výsledkov vyberte položku **Správca zariadení**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="9da8c-112">V časti **Batérie** kliknite pravým tlačidlom myši na batériu zariadenia, kliknite na položku **Zakázať** a potom na položku **Áno**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="9da8c-113">Počkajte niekoľko sekúnd, kliknite pravým tlačidlom myši na batériu a kliknite na položku **Povoliť**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="9da8c-114">Potom reštartujte zariadenie.</span><span class="sxs-lookup"><span data-stu-id="9da8c-114">Then restart your device.</span></span>

<span data-ttu-id="9da8c-115">Ak ste postupovali podľa uvedených pokynov, ale ikona batérie sa na paneli úloh nezobrazuje, do vyhľadávacieho poľa na paneli úloh napíšte výraz **správca úloh** a potom v zozname výsledkov kliknite na položku **Správca úloh**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="9da8c-116">Na karte **Procesy** v stĺpci časti **Názov** kliknite pravým tlačidlom myši na položku **Prieskumník** a potom kliknite na položku **Reštartovať**.</span><span class="sxs-lookup"><span data-stu-id="9da8c-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
