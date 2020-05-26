---
title: Spustenie nástroja Windows Diagnostika pamäte v systéme Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358295"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="28663-102">Spustenie nástroja Windows Diagnostika pamäte v systéme Windows 10</span><span class="sxs-lookup"><span data-stu-id="28663-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="28663-103">Ak systém Windows a aplikácie v počítači zlyhajú, zmrazujú alebo pôsobia nestabilným spôsobom, môže sa stať, že máte problém s pamäťou počítača (RAM).</span><span class="sxs-lookup"><span data-stu-id="28663-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="28663-104">Môžete spustiť Windows Diagnostika pamäte na kontrolu problémov s PC RAM.</span><span class="sxs-lookup"><span data-stu-id="28663-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="28663-105">Do vyhľadávacieho poľa na paneli úloh zadajte príkaz **Diagnostika pamäte**a potom vyberte položku **Windows Diagnostika pamäte**.</span><span class="sxs-lookup"><span data-stu-id="28663-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="28663-106">Ak chcete spustiť diagnostický, PC je potrebné reštartovať.</span><span class="sxs-lookup"><span data-stu-id="28663-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="28663-107">Máte možnosť reštartovať okamžite (prosím uložte svoju prácu a zatvorte otvorené dokumenty a e-maily ako prvý), alebo naplánovať diagnostické spustiť automaticky pri ďalšom reštartovaní počítača:</span><span class="sxs-lookup"><span data-stu-id="28663-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Diagnostika pamäte](media/windows-memory-diagnostic.png)

<span data-ttu-id="28663-109">Po reštartovaní počítača sa **nástroj Windows Diagnostika pamäte** spustí automaticky.</span><span class="sxs-lookup"><span data-stu-id="28663-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="28663-110">Stav a priebeh sa zobrazí ako diagnostický beh a máte možnosť zrušiť diagnostiku stlačením klávesu **ESC** na klávesnici.</span><span class="sxs-lookup"><span data-stu-id="28663-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="28663-111">Po dokončení diagnostiky sa systém Windows spustí normálne.</span><span class="sxs-lookup"><span data-stu-id="28663-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="28663-112">Ihneď po reštarte, keď sa zobrazí pracovná plocha, zobrazí sa upozornenie (vedľa ikony **centra akcií** na paneli úloh), aby ste uviedli, či sa našli chyby pamäte.</span><span class="sxs-lookup"><span data-stu-id="28663-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="28663-113">Príklad:</span><span class="sxs-lookup"><span data-stu-id="28663-113">For example:</span></span>

<span data-ttu-id="28663-114">Tu je ikona centra akcií:</span><span class="sxs-lookup"><span data-stu-id="28663-114">Here's the Action Center icon:</span></span> ![Ikona centra akcií](media/action-center-icon.png) 

<span data-ttu-id="28663-116">A vzorové oznámenie:</span><span class="sxs-lookup"><span data-stu-id="28663-116">And a sample notification:</span></span> ![Žiadne chyby pamäte](media/no-memory-errors.png)

<span data-ttu-id="28663-118">Ak ste oznámenie vynechali, môžete na paneli úloh vybrať ikonu **centra akcií** , aby sa zobrazil **centrum akcií** a zobrazí sa posúvateľný zoznam upozornení.</span><span class="sxs-lookup"><span data-stu-id="28663-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="28663-119">Ak chcete skontrolovať podrobné informácie, zadajte **udalosť** do vyhľadávacieho poľa na paneli úloh a potom vyberte položku **Zobrazovač udalostí**.</span><span class="sxs-lookup"><span data-stu-id="28663-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="28663-120">V table **Zobrazovač udalostí**na ľavej strane prejdite na **denníky systému Windows > systém**.</span><span class="sxs-lookup"><span data-stu-id="28663-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="28663-121">Na pravej table prehľadá zoznam pri pohľade na **zdrojový** stĺpec, až uvidíte udalosti s zdrojovú hodnotu **memorydiagnostics-výsledky**.</span><span class="sxs-lookup"><span data-stu-id="28663-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="28663-122">Zvýraznite každú takúto udalosť a pozrite si informácie o výsledku v poli na karte **Všeobecné** pod zoznamom.</span><span class="sxs-lookup"><span data-stu-id="28663-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
