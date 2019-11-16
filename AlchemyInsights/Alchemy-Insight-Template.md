---
title: rovnaký názov súboru je najlepší
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800060"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="e7412-102">Povinné alchýmia Hlavička H1, H2's nefungujú.</span><span class="sxs-lookup"><span data-stu-id="e7412-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="e7412-103">Osvedčené postupy a usmernenia pre alchýmia Authoring:</span><span class="sxs-lookup"><span data-stu-id="e7412-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="e7412-104">**Nepoužívajte hniezdo Alchemy postrehy v priečinkoch**-to bude prestávka URL štruktúru.</span><span class="sxs-lookup"><span data-stu-id="e7412-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="e7412-105">Hľadáme do stanovenia tohto.</span><span class="sxs-lookup"><span data-stu-id="e7412-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="e7412-106">Súbory v priečinku **Alchemyinpamiatkam** by mali mať malé názvy súborov s pomlčkami pre medzery ex.</span><span class="sxs-lookup"><span data-stu-id="e7412-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="e7412-107">***ako-to-Enable-Litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="e7412-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="e7412-108">Zahrnúť ID pravidla alebo identifikátor vedierko z [Alchemy partner Portal](https://alchemyportal.azurewebsites.net) v MS. Custom pole.</span><span class="sxs-lookup"><span data-stu-id="e7412-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="e7412-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="e7412-109">ex.</span></span> <span data-ttu-id="e7412-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="e7412-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="e7412-111">Použite zvyšok metaúdajov v hornej časti tohto súboru ako šablónu.</span><span class="sxs-lookup"><span data-stu-id="e7412-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="e7412-112">V [Alchemy partner Portal](https://alchemyportal.azurewebsites.net), prejdite nadol na sekciu **Zákazník Insight názov:** a použiť, že ako východiskový bod pre váš H1 titul pre pochopenie.</span><span class="sxs-lookup"><span data-stu-id="e7412-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="e7412-113">Alchýmia postrehy musia mať len jeden H1 v hornej alebo budú zlomiť vo výrobe.</span><span class="sxs-lookup"><span data-stu-id="e7412-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="e7412-114">H2s nespôsobujú ani tak použiť **tučné** alebo iné konvencie znamenať samostatných sekcií.</span><span class="sxs-lookup"><span data-stu-id="e7412-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="e7412-115">Potom vyplňte základný text pomocou návrhu materiálu v sekcii prehľady zákazníkov na stránke pravidla alchýmie</span><span class="sxs-lookup"><span data-stu-id="e7412-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="e7412-116">Zoznamy s odrážkami sú v poriadku</span><span class="sxs-lookup"><span data-stu-id="e7412-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="e7412-117">Číslované zoznamy príliš</span><span class="sxs-lookup"><span data-stu-id="e7412-117">Numbered lists too</span></span>
    1. <span data-ttu-id="e7412-118">**Tučné** a *kurzíva* sú a-OK</span><span class="sxs-lookup"><span data-stu-id="e7412-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="e7412-119">Odkazy by mali byť vždy buď **"Odkazy na web"/externé** alebo **hlboké-odkazy na prvky používateľského rozhrania**, nie interné odkazy.</span><span class="sxs-lookup"><span data-stu-id="e7412-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="e7412-120">Obrázky nie sú oficiálne podporované v tejto dobe, ale je to na pláne.</span><span class="sxs-lookup"><span data-stu-id="e7412-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="e7412-121">A to je naozaj už trochu príliš dlho.</span><span class="sxs-lookup"><span data-stu-id="e7412-121">And this is really already a bit too long.</span></span> <span data-ttu-id="e7412-122">Najlepšia prax je asi 400 znakov---------------------------------</span><span class="sxs-lookup"><span data-stu-id="e7412-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="e7412-123">Akonáhle je váš obsah pripravený, vytiahnite ho do živej pobočky.</span><span class="sxs-lookup"><span data-stu-id="e7412-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="e7412-124">Potom prejdite na [portál Alchemy partnera](https://alchemyportal.azurewebsites.net) a zadajte názov súboru do poľa Adresa URL.</span><span class="sxs-lookup"><span data-stu-id="e7412-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 