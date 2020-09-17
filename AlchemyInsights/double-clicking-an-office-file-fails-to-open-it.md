---
title: Dvojitým kliknutím na súbor balíka Office sa daný súbor nedokáže otvoriť
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812094"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="b604c-102">Dvojitým kliknutím na súbor balíka Office sa daný súbor nedokáže otvoriť</span><span class="sxs-lookup"><span data-stu-id="b604c-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="b604c-103">Po dvojitom kliknutí na súbor balíka Office sa môže zobraziť program otvoriť, ale samotný súbor sa neotvorí.</span><span class="sxs-lookup"><span data-stu-id="b604c-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="b604c-104">Alebo sa môže zobraziť chybové hlásenie: Vyskytol sa problém s odoslaním príkazu do programu.</span><span class="sxs-lookup"><span data-stu-id="b604c-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="b604c-105">K dispozícii je veľa príčin, ale dva najbežnejšie riešenia:</span><span class="sxs-lookup"><span data-stu-id="b604c-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="b604c-106">V programe Excel skontrolujte, či je možnosť DDE nekontrolovaná.</span><span class="sxs-lookup"><span data-stu-id="b604c-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="b604c-107">Možnosť možno nájsť vytvorením nového zošita a výberom **možnosti > súboru > rozšírené**.</span><span class="sxs-lookup"><span data-stu-id="b604c-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="b604c-108">V časti **Všeobecné** začiarknite políčko **Ignorovať iné aplikácie, ktoré používajú dynamickú výmenu údajov (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="b604c-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="b604c-109">Ak chcete obnoviť predvolené nastavenia, spustite online opravu.</span><span class="sxs-lookup"><span data-stu-id="b604c-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="b604c-110">Kliknite na tlačidlo Štart systému Windows a vyhľadajte položku Ovládací panel.</span><span class="sxs-lookup"><span data-stu-id="b604c-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="b604c-111">Otvorte **Ovládací panel**a prejdite na položky **programy > programy a súčasti**.</span><span class="sxs-lookup"><span data-stu-id="b604c-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="b604c-112">Kliknite pravým tlačidlom myši na položku **Microsoft Office [verzia]** a vyberte položku **zmeniť > online opravu**.</span><span class="sxs-lookup"><span data-stu-id="b604c-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="b604c-113">Ak ani jedna z týchto riešení nie je k dispozícii, v článku technickej podpory môžete nájsť podrobnejší zoznam riešení, [dvojitým kliknutím na súbor balíka Office ho nedokáže otvoriť](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="b604c-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
