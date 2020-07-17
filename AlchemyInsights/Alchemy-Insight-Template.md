---
title: rovnako ako názov súboru je najlepšie
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750985"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="6d8e4-102">"Požadovaná alchýmia hlavička H1, H2 to nefunguje."</span><span class="sxs-lookup"><span data-stu-id="6d8e4-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="6d8e4-103">Osvedčené postupy a usmernenia pre tvorbu alchýmie:</span><span class="sxs-lookup"><span data-stu-id="6d8e4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="6d8e4-104">**Nehniezditi Alchemy Postrehy v priečinkoch**- to bude zlomiť url štruktúru.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="6d8e4-105">Snažíme sa to napraviť.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="6d8e4-106">Súbory v priečinku **AlchemyInsights** by mali mať malé názvy súborov s pomlčkami pre medzery ex.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="6d8e4-107">***na zadržanie súdnych sporov***.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="6d8e4-108">Do poľa ms.custom zahrňte identifikáciu pravidla alebo identifikátor sektora z [portálu partnera Alchemy.](https://alchemyportal.azurewebsites.net)</span><span class="sxs-lookup"><span data-stu-id="6d8e4-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="6d8e4-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-109">ex.</span></span> <span data-ttu-id="6d8e4-110">***ms.custom: 100021 ms.custom: 100021 ms.custom: 100021 ms***</span><span class="sxs-lookup"><span data-stu-id="6d8e4-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="6d8e4-111">Ako šablónu použite ostatné metaúdaje v hornej časti tohto súboru.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="6d8e4-112">Na [portáli Alchemy Partner](https://alchemyportal.azurewebsites.net)prejdite do časti **Názov prehľadu zákazníkov:** a použite ho ako východiskový bod pre váš titul H1 na prehľad.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="6d8e4-113">Alchýmia Postrehy musia mať len jeden H1 na vrchole, alebo sa zlomiť vo výrobe.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="6d8e4-114">H2s nerobia buď tak použiť **tučné** alebo iné konvencie znamenať samostatné sekcie.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="6d8e4-115">Potom vyplňte základný text pomocou konceptu materiálu v časti Prehľady zákazníkov na stránke Pravidlo alchýmie</span><span class="sxs-lookup"><span data-stu-id="6d8e4-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="6d8e4-116">Zoznamy s odrážkami sú v poriadku</span><span class="sxs-lookup"><span data-stu-id="6d8e4-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="6d8e4-117">Číslované zoznamy príliš</span><span class="sxs-lookup"><span data-stu-id="6d8e4-117">Numbered lists too</span></span>
    1. <span data-ttu-id="6d8e4-118">**Tučné** a *kurzíva* sú-ok</span><span class="sxs-lookup"><span data-stu-id="6d8e4-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="6d8e4-119">Odkazy by mali byť vždy buď **"odkazy na web"/ externé** alebo **hlboké-odkazy na prvky UI**, nie vnútorné odkazy.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="6d8e4-120">Obrázky nie sú oficiálne podporované v tejto dobe, ale je to na pláne.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="6d8e4-121">A to je naozaj už trochu príliš dlho.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-121">And this is really already a bit too long.</span></span> <span data-ttu-id="6d8e4-122">Osvedčené postupy sú asi 400 znakov ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="6d8e4-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="6d8e4-123">Akonáhle je váš obsah je pripravený, vytiahnite ho do live pobočky.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="6d8e4-124">Potom prejdite na [portál Alchemy Partner](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa url.</span><span class="sxs-lookup"><span data-stu-id="6d8e4-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 