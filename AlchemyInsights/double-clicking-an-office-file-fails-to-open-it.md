---
title: Dvojitým kliknutím na súbor balíka Office sa súbor neotvorí
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814820"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="8c979-102">Dvojitým kliknutím na súbor balíka Office sa súbor neotvorí</span><span class="sxs-lookup"><span data-stu-id="8c979-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="8c979-103">Po dvojitom kliknutí na súbor balíka Office sa môže zobraziť, že program je otvorený, ale samotný súbor sa neotvorí.</span><span class="sxs-lookup"><span data-stu-id="8c979-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="8c979-104">Alebo sa môže zobraziť chybové hlásenie: Vyskytol sa problém s odoslaním príkazu do programu.</span><span class="sxs-lookup"><span data-stu-id="8c979-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="8c979-105">Toto má mnoho príčin, ale dve najbežnejšie riešenia sú:</span><span class="sxs-lookup"><span data-stu-id="8c979-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="8c979-106">V Exceli skontrolujte, či nie je vybratá možnosť DDE.</span><span class="sxs-lookup"><span data-stu-id="8c979-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="8c979-107">Túto možnosť môžete nájsť vytvorením nového zošita a výberom položky Súbor > **Možnosti > Rozšírené**.</span><span class="sxs-lookup"><span data-stu-id="8c979-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="8c979-108">V časti **Všeobecné** zrušte začiarknutie políčka **Ignorovať ostatné aplikácie, ktoré používajú dynamickú výmenu údajov (DDE).**</span><span class="sxs-lookup"><span data-stu-id="8c979-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="8c979-109">Spustite online opravu a obnovte predvolené nastavenia.</span><span class="sxs-lookup"><span data-stu-id="8c979-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="8c979-110">Kliknite na tlačidlo Štart vo Windowse a vyhľadajte položku Ovládací panel.</span><span class="sxs-lookup"><span data-stu-id="8c979-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="8c979-111">Otvorte Ovládací **panel a** prejdite na položku Programy > Programy **a súčasti.**</span><span class="sxs-lookup"><span data-stu-id="8c979-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="8c979-112">Potom kliknite pravým tlačidlom myši **na položku Microsoft Office [Verzia]** a vyberte položku zmeniť > online **oprava.**</span><span class="sxs-lookup"><span data-stu-id="8c979-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="8c979-113">Ak ani jedno z týchto riešení nefunguje, v článku podpory nájdete úplne väčší zoznam riešení. Dvojitým kliknutím na súbor balíka Office sa súbor [neotvorí.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="8c979-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
