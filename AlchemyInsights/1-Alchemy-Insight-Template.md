---
title: 'rovnaký ako názov súboru je najlepšie [pravidlo #-Popis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662945"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="734b6-102">Požadované zákazníkom čelia H1, H2 nefunguje</span><span class="sxs-lookup"><span data-stu-id="734b6-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="734b6-103">Príklad textu blok - postupujte podľa týchto pokynov:</span><span class="sxs-lookup"><span data-stu-id="734b6-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="734b6-104">Súbory v priečinku **AlchemyInsights** by mali mať identifikácia pravidla a pravidlo názov z [alchýmie Partner portálu](https://alchemyportal.azurewebsites.net) v názve súboru.</span><span class="sxs-lookup"><span data-stu-id="734b6-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="734b6-p101">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="734b6-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="734b6-p102">Metadáta použiť v hornej časti tento súbor ako šablónu. Nič iné nevyžaduje.</span><span class="sxs-lookup"><span data-stu-id="734b6-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="734b6-109">[Alchýmia Partner portal](https://alchemyportal.azurewebsites.net)prejdite nadol do sekcie **zákazníka Insight titul:** a použiť ho ako východiskový bod pre nadpis H1 pre pochopenie.</span><span class="sxs-lookup"><span data-stu-id="734b6-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="734b6-p103">Alchýmia poznatky musí mať iba jeden H1 navrchu alebo bude prestávka vo výrobe. H2s neznemožňujú tak použiť **tučné** alebo iných dohovorov znamenať samostatných sekcií.</span><span class="sxs-lookup"><span data-stu-id="734b6-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="734b6-112">Ďalšie, vyplňte základný text pomocou návrh materiálu v časti prehľady o zákazníkoch alchýmia pravidlo stránky</span><span class="sxs-lookup"><span data-stu-id="734b6-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="734b6-113">Zoznamy s odrážkami sú v poriadku</span><span class="sxs-lookup"><span data-stu-id="734b6-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="734b6-114">Číslované zoznamy príliš</span><span class="sxs-lookup"><span data-stu-id="734b6-114">Numbered lists too</span></span>
    1. <span data-ttu-id="734b6-115">**Tučné písmo** a *kurzíva* sú a-ok</span><span class="sxs-lookup"><span data-stu-id="734b6-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="734b6-116">Odkazy by mali byť vždy buď **"Odkazy na web" / externý** alebo **hlboko-odkazy na prvky používateľského rozhrania**, nie interné odkazy.</span><span class="sxs-lookup"><span data-stu-id="734b6-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="734b6-p104">A to je naozaj už trochu príliš dlho. Najlepšie je asi 400 znakov---</span><span class="sxs-lookup"><span data-stu-id="734b6-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="734b6-p105">Akonáhle váš obsah je pripravený, vytiahnite ju na živé vetvy. Potom [alchýmia Partner portálu](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url. Uistite sa, že pohľad Review a publikovanej hovorí "áno" a kliknite na tlačidlo pravidlo pre aktualizáciu. (To bude vyzerať hezčí v novej verzii portálu - uvoľnenie čoskoro.)</span><span class="sxs-lookup"><span data-stu-id="734b6-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL poľa](media/for-content-team.PNG)

