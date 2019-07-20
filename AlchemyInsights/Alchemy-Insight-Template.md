---
title: Najlepšie je rovnaký ako názov súboru
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800060"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="984f0-102">Vyžaduje alchýmie hlavičke H1, H2-nefungujú.</span><span class="sxs-lookup"><span data-stu-id="984f0-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="984f0-103">Najlepšie postupy a pokyny pre authoring alchýmia:</span><span class="sxs-lookup"><span data-stu-id="984f0-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="984f0-104">**Nest alchýmia postrehy v priečinkoch**- to bude prestávka v url štruktúru.</span><span class="sxs-lookup"><span data-stu-id="984f0-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="984f0-105">Hľadáme do stanovenie tejto.</span><span class="sxs-lookup"><span data-stu-id="984f0-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="984f0-106">Súbory v priečinku **AlchemyInsights** by mali mať malé písmená názvov súborov s pomlčkami medzery ex.</span><span class="sxs-lookup"><span data-stu-id="984f0-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="984f0-107">***jak-na-enable--zadržanie***.</span><span class="sxs-lookup"><span data-stu-id="984f0-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="984f0-108">Zahŕňajú identifikácia pravidla alebo vedierko ID z [alchýmie Partner portal](https://alchemyportal.azurewebsites.net) v poli ms.custom.</span><span class="sxs-lookup"><span data-stu-id="984f0-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="984f0-109">ex.</span><span class="sxs-lookup"><span data-stu-id="984f0-109">ex.</span></span> <span data-ttu-id="984f0-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="984f0-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="984f0-111">Použite zvyšok metaúdaje v hornej časti tohto súboru ako šablóny.</span><span class="sxs-lookup"><span data-stu-id="984f0-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="984f0-112">[Alchýmia Partner portal](https://alchemyportal.azurewebsites.net)prejdite nadol do sekcie **zákazníka Insight titul:** a použiť ho ako východiskový bod pre nadpis H1 pre pochopenie.</span><span class="sxs-lookup"><span data-stu-id="984f0-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="984f0-113">Alchýmia poznatky musí mať iba jeden H1 navrchu alebo bude prestávka vo výrobe.</span><span class="sxs-lookup"><span data-stu-id="984f0-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="984f0-114">H2s neznemožňujú tak použiť **tučné** alebo iných dohovorov znamenať samostatných sekcií.</span><span class="sxs-lookup"><span data-stu-id="984f0-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="984f0-115">Ďalšie, vyplňte základný text pomocou návrh materiálu v časti prehľady o zákazníkoch alchýmia pravidlo stránky</span><span class="sxs-lookup"><span data-stu-id="984f0-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="984f0-116">Zoznamy s odrážkami sú v poriadku</span><span class="sxs-lookup"><span data-stu-id="984f0-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="984f0-117">Číslované zoznamy príliš</span><span class="sxs-lookup"><span data-stu-id="984f0-117">Numbered lists too</span></span>
    1. <span data-ttu-id="984f0-118">**Tučné písmo** a *kurzíva* sú a-ok</span><span class="sxs-lookup"><span data-stu-id="984f0-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="984f0-119">Odkazy by mali byť vždy buď **"Odkazy na web" / externý** alebo **hlboko-odkazy na prvky používateľského rozhrania**, nie interné odkazy.</span><span class="sxs-lookup"><span data-stu-id="984f0-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="984f0-120">Obrázky nie sú oficiálne podporované v tejto dobe, ale to je na pláne.</span><span class="sxs-lookup"><span data-stu-id="984f0-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="984f0-121">A to je naozaj už trochu príliš dlho.</span><span class="sxs-lookup"><span data-stu-id="984f0-121">And this is really already a bit too long.</span></span> <span data-ttu-id="984f0-122">Najlepšie je asi 400 znakov---</span><span class="sxs-lookup"><span data-stu-id="984f0-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="984f0-123">Akonáhle váš obsah je pripravený, vytiahnite ju na živé vetvy.</span><span class="sxs-lookup"><span data-stu-id="984f0-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="984f0-124">Potom [alchýmia Partner portálu](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url.</span><span class="sxs-lookup"><span data-stu-id="984f0-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 