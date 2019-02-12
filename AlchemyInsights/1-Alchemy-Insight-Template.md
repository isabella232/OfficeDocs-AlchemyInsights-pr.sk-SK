---
title: 'rovnaký ako názov súboru je najlepšie [pravidlo #-Popis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939322"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="a9083-102">Vyžaduje alchýmie hlavičke H1, H2-nefungujú.</span><span class="sxs-lookup"><span data-stu-id="a9083-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="a9083-103">Najlepšie postupy a pokyny pre authoring alchýmia:</span><span class="sxs-lookup"><span data-stu-id="a9083-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="a9083-p101">**Nest alchýmia postrehy v priečinkoch**- to bude prestávka v url štruktúru. Hľadáme do stanovenie tejto.</span><span class="sxs-lookup"><span data-stu-id="a9083-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="a9083-106">Súbory v priečinku **AlchemyInsights** by mali mať identifikácia pravidla a pravidlo názov z [alchýmie Partner portálu](https://alchemyportal.azurewebsites.net) v názve súboru.</span><span class="sxs-lookup"><span data-stu-id="a9083-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="a9083-p102">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="a9083-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="a9083-p103">Metadáta použiť v hornej časti tento súbor ako šablónu. Nič iné nevyžaduje.</span><span class="sxs-lookup"><span data-stu-id="a9083-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="a9083-111">[Alchýmia Partner portal](https://alchemyportal.azurewebsites.net)prejdite nadol do sekcie **zákazníka Insight titul:** a použiť ho ako východiskový bod pre nadpis H1 pre pochopenie.</span><span class="sxs-lookup"><span data-stu-id="a9083-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="a9083-p104">Alchýmia poznatky musí mať iba jeden H1 navrchu alebo bude prestávka vo výrobe. H2s neznemožňujú tak použiť **tučné** alebo iných dohovorov znamenať samostatných sekcií.</span><span class="sxs-lookup"><span data-stu-id="a9083-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="a9083-114">Ďalšie, vyplňte základný text pomocou návrh materiálu v časti prehľady o zákazníkoch alchýmia pravidlo stránky</span><span class="sxs-lookup"><span data-stu-id="a9083-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="a9083-115">Zoznamy s odrážkami sú v poriadku</span><span class="sxs-lookup"><span data-stu-id="a9083-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="a9083-116">Číslované zoznamy príliš</span><span class="sxs-lookup"><span data-stu-id="a9083-116">Numbered lists too</span></span>
    1. <span data-ttu-id="a9083-117">**Tučné písmo** a *kurzíva* sú a-ok</span><span class="sxs-lookup"><span data-stu-id="a9083-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="a9083-118">Odkazy by mali byť vždy buď **"Odkazy na web" / externý** alebo **hlboko-odkazy na prvky používateľského rozhrania**, nie interné odkazy.</span><span class="sxs-lookup"><span data-stu-id="a9083-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="a9083-p105">A to je naozaj už trochu príliš dlho. Najlepšie je asi 400 znakov---</span><span class="sxs-lookup"><span data-stu-id="a9083-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="a9083-p106">Akonáhle váš obsah je pripravený, vytiahnite ju na živé vetvy. Potom [alchýmia Partner portálu](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url. Uistite sa, že pohľad Review a publikovanej hovorí "áno" a kliknite na tlačidlo pravidlo pre aktualizáciu. **(To bude vyzerať hezčí v novej verzii portálu - uvoľnenie čoskoro.)** 
 ![url poľa](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="a9083-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

