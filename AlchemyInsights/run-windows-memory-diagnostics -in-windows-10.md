---
title: Spustenie diagnostiky pamäte Windowsu vo Windowse 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826682"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="b5eda-102">Spustenie diagnostiky pamäte Windowsu vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="b5eda-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="b5eda-103">Ak Windows a aplikácie v počítači zlyhávajú, zamŕzajú alebo pôsobia nestabilným spôsobom, môže ísť o problém s pamäťou PC (RAM).</span><span class="sxs-lookup"><span data-stu-id="b5eda-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="b5eda-104">Môžete spustiť nástroj Diagnostika pamäte Windowsu a zistiť, či sa v počítači nenálili problémy s pamäťou RAM počítača.</span><span class="sxs-lookup"><span data-stu-id="b5eda-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="b5eda-105">Do vyhľadávacieho poľa na paneli úloh zadajte výraz **Diagnostika pamäte** a potom vyberte položku **Diagnostika pamäte systému Windows.**</span><span class="sxs-lookup"><span data-stu-id="b5eda-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="b5eda-106">Na spustenie diagnostiky musí byť počítač reštartovaný.</span><span class="sxs-lookup"><span data-stu-id="b5eda-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="b5eda-107">Máte možnosť okamžite reštartovať (najprv uložte svoju prácu a zatvorte otvorené dokumenty a e-maily) alebo naplánujte spustenie diagnostiky automaticky pri ďalšom reštartovaní počítača:</span><span class="sxs-lookup"><span data-stu-id="b5eda-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Nástroj Windows Diagnostika pamäte](media/windows-memory-diagnostic.png)

<span data-ttu-id="b5eda-109">Po reštartovaní počítača sa **nástroj Windows Diagnostika pamäte** spustí automaticky.</span><span class="sxs-lookup"><span data-stu-id="b5eda-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="b5eda-110">Stav a priebeh sa budú zobrazovať pri spustení diagnostiky a máte možnosť zrušiť diagnostiku stlačením klávesu **ESC** na klávesnici.</span><span class="sxs-lookup"><span data-stu-id="b5eda-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="b5eda-111">Po dokončení diagnostiky sa Windows spustí normálne.</span><span class="sxs-lookup"><span data-stu-id="b5eda-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="b5eda-112">Po reštartovaní sa hneď po reštartovaní zobrazí oznámenie  (vedľa ikony Centrum akcií na paneli úloh), ktoré informuje, či sa našli nejaké chyby pamäte.</span><span class="sxs-lookup"><span data-stu-id="b5eda-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="b5eda-113">Príklad:</span><span class="sxs-lookup"><span data-stu-id="b5eda-113">For example:</span></span>

<span data-ttu-id="b5eda-114">Tu je ikona Centra akcií:</span><span class="sxs-lookup"><span data-stu-id="b5eda-114">Here's the Action Center icon:</span></span> ![Ikona Centra akcií](media/action-center-icon.png) 

<span data-ttu-id="b5eda-116">A vzorové oznámenie:</span><span class="sxs-lookup"><span data-stu-id="b5eda-116">And a sample notification:</span></span> ![Žiadne chyby pamäte](media/no-memory-errors.png)

<span data-ttu-id="b5eda-118">Ak ste oznámenie nestihli,  môžete vybrať ikonu Centra  akcií na paneli úloh a zobraziť centrum akcií a zobraziť posúvateľný zoznam oznámení.</span><span class="sxs-lookup"><span data-stu-id="b5eda-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="b5eda-119">Ak chcete skontrolovať podrobné informácie, **do** vyhľadávacieho poľa na paneli úloh zadajte udalosť a potom vyberte položku **Zobrazovač udalostí**.</span><span class="sxs-lookup"><span data-stu-id="b5eda-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="b5eda-120">Na **ľavej table** zobrazovača udalostí prejdite na položku **Denníky Windowsu > systému**.</span><span class="sxs-lookup"><span data-stu-id="b5eda-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="b5eda-121">Na pravej table si pri pohľade na  stĺpec Zdroj pozrite zoznam nadol, až kým sa nenájde udalosť s hodnotou Source value **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="b5eda-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="b5eda-122">Zvýraznite každú takúto udalosť a v poli na karte Všeobecné pod **zoznamom** zobrazte informácie o výsledku.</span><span class="sxs-lookup"><span data-stu-id="b5eda-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
