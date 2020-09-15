---
title: rovnako ako názov súboru je najvhodnejší
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664149"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="da0d5-102">"Požadovaná alchýmia header H1, H2's nefungujú."</span><span class="sxs-lookup"><span data-stu-id="da0d5-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="da0d5-103">Najvhodnejšie postupy a pokyny na vytváranie alchýmie:</span><span class="sxs-lookup"><span data-stu-id="da0d5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="da0d5-104">Do **not Nest alchýmia prehľady v priečinkoch**– tým sa preruší štruktúra URL adresy.</span><span class="sxs-lookup"><span data-stu-id="da0d5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="da0d5-105">My sme hľadali riešenie tohto.</span><span class="sxs-lookup"><span data-stu-id="da0d5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="da0d5-106">Súbory v priečinku **AlchemyInsights** by mali obsahovať malé názvy súborov s pomlčkami pre medzery ex.</span><span class="sxs-lookup"><span data-stu-id="da0d5-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="da0d5-107">***postup – povolenie – zadržanie***.</span><span class="sxs-lookup"><span data-stu-id="da0d5-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="da0d5-108">Zahrňte ID pravidla alebo identifikáciu vedierko z [partnerského portálu alchýmie](https://alchemyportal.azurewebsites.net) do poľa MS. custom.</span><span class="sxs-lookup"><span data-stu-id="da0d5-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="da0d5-109">napríklad.</span><span class="sxs-lookup"><span data-stu-id="da0d5-109">ex.</span></span> <span data-ttu-id="da0d5-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="da0d5-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="da0d5-111">Použite zvyšok metaúdajov v hornej časti tohto súboru ako šablónu.</span><span class="sxs-lookup"><span data-stu-id="da0d5-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="da0d5-112">Na [partnerskom portáli alchýmie](https://alchemyportal.azurewebsites.net)prejdite nadol na časť **názov prehľadu zákazníka:** a použite ho ako východiskový bod pre názov H1 pre prehľad.</span><span class="sxs-lookup"><span data-stu-id="da0d5-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="da0d5-113">Podrobné informácie o alchýmii musia mať v hornej časti iba jeden H1 alebo sa rozkladajú vo výrobe.</span><span class="sxs-lookup"><span data-stu-id="da0d5-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="da0d5-114">H2s Nekresliť ani tak použite **tučné písmo** alebo iné konvencie označujúce samostatné sekcie.</span><span class="sxs-lookup"><span data-stu-id="da0d5-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="da0d5-115">Potom vyplňte základný text pomocou konceptu materiál v časti prehľady zákazníkov na stránke pravidiel alchýmie.</span><span class="sxs-lookup"><span data-stu-id="da0d5-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="da0d5-116">Zoznamy s odrážkami sú v pohodě</span><span class="sxs-lookup"><span data-stu-id="da0d5-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="da0d5-117">Číslované zoznamy</span><span class="sxs-lookup"><span data-stu-id="da0d5-117">Numbered lists too</span></span>
    1. <span data-ttu-id="da0d5-118">**Tučné písmo** a *kurzíva* sú a-OK</span><span class="sxs-lookup"><span data-stu-id="da0d5-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="da0d5-119">Prepojenia by mali byť vždy buď **"prepojenia na web"/external** alebo **hlboké prepojenia na prvky používateľského rozhrania**, nie interné prepojenia.</span><span class="sxs-lookup"><span data-stu-id="da0d5-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="da0d5-120">Obrázky nie sú v súčasnosti oficiálne podporované, ale je to na pláne.</span><span class="sxs-lookup"><span data-stu-id="da0d5-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="da0d5-121">A to je naozaj už trochu príliš dlho.</span><span class="sxs-lookup"><span data-stu-id="da0d5-121">And this is really already a bit too long.</span></span> <span data-ttu-id="da0d5-122">Najvhodnejšie postupy sú približne 400 znakov---------------------------------</span><span class="sxs-lookup"><span data-stu-id="da0d5-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="da0d5-123">Keď je váš obsah pripravený, presuňte ho do živej vetvy.</span><span class="sxs-lookup"><span data-stu-id="da0d5-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="da0d5-124">Potom prejdite na [partnerský portál alchýmie](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa URL adresa.</span><span class="sxs-lookup"><span data-stu-id="da0d5-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 