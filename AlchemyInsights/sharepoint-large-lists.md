---
title: Veľké zoznamy lokality SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488532"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="efda3-102">Práca s veľkými zoznamami a knižnicami v SharePointe</span><span class="sxs-lookup"><span data-stu-id="efda3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="efda3-103">Zoznamy a knižnice lokality SharePoint môžu obsahovať až 30 000 000 položiek, ale keď majú viac ako 5 000 položiek, pri pokuse o prácu s nimi sa môže zobraziť prahová chyba zobrazenia zoznamu.</span><span class="sxs-lookup"><span data-stu-id="efda3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="efda3-104">Tento prah je zavedený na udržanie výkonnosti služby.</span><span class="sxs-lookup"><span data-stu-id="efda3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="efda3-105">Nedá sa zmeniť.</span><span class="sxs-lookup"><span data-stu-id="efda3-105">It can't be changed.</span></span> <span data-ttu-id="efda3-106">Aby sa predišlo nárazu tejto prahovej hodnoty:</span><span class="sxs-lookup"><span data-stu-id="efda3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="efda3-107">**Používať moderné**</span><span class="sxs-lookup"><span data-stu-id="efda3-107">**Use modern**</span></span>

<span data-ttu-id="efda3-108">Zobrazenia zobrazujúce veľa položiek fungujú najlepšie v modernom zážitku.</span><span class="sxs-lookup"><span data-stu-id="efda3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="efda3-109">[Využite moderné skúsenosti](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , aby ste sa vyhli chybám, ktoré by ste mohli vidieť v klasickom zážitku.</span><span class="sxs-lookup"><span data-stu-id="efda3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="efda3-110">**Pridať indexy**</span><span class="sxs-lookup"><span data-stu-id="efda3-110">**Add indexes**</span></span>

<span data-ttu-id="efda3-111">Keď filtrujete alebo zoradíte podľa stĺpca, ktorý nemá index, môže sa zobraziť chybové hlásenie.</span><span class="sxs-lookup"><span data-stu-id="efda3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="efda3-112">[Pridať index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ručne z **nastavenia zoznamu** v menu nastavenia, potom **indexované stĺpce**.</span><span class="sxs-lookup"><span data-stu-id="efda3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="efda3-113">**Úprava zobrazenia zoznamu**</span><span class="sxs-lookup"><span data-stu-id="efda3-113">**Edit the list view**</span></span>

<span data-ttu-id="efda3-114">Ak sa pri práci s veľkým zoznamom vyskytne chyba, [Upravte zobrazenie zoznamu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="efda3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="efda3-115">Nasledujúce štyri zmeny odstránia prah zobrazenia zoznamu chyby.</span><span class="sxs-lookup"><span data-stu-id="efda3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="efda3-116">Vykonajte všetky štyri zmeny odstrániť všetky chyby.</span><span class="sxs-lookup"><span data-stu-id="efda3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="efda3-117">Ak sa stále zobrazujú chyby, skontrolujte [spravovanie veľkých zoznamov a knižníc](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="efda3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="efda3-118">Vyberte položku **žiadne** z **prvého zoradenia podľa stĺpca** a **potom zoradiť podľa stĺpca**.</span><span class="sxs-lookup"><span data-stu-id="efda3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="efda3-119">**V stĺpci** vyberte položku **žiadne** z prvej skupiny a **potom zoskupte podľa stĺpca**.</span><span class="sxs-lookup"><span data-stu-id="efda3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="efda3-120">V časti **súčty** vyberte možnosť **žiadne** pre všetky stĺpce.</span><span class="sxs-lookup"><span data-stu-id="efda3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="efda3-121">Zrušte výber všetkých stĺpcov, ale pre zobrazenie z časti **stĺpce** .</span><span class="sxs-lookup"><span data-stu-id="efda3-121">Deselect all but one column for display from the **Columns** section.</span></span>

