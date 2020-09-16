---
title: Veľké zoznamy v SharePointe
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720148"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="5ded8-102">Práca s veľkými zoznamami a knižnicami v SharePointe</span><span class="sxs-lookup"><span data-stu-id="5ded8-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="5ded8-103">Zoznamy a knižnice SharePointu môžu obsahovať až 30 000 000 položiek, ale keď majú viac ako 5 000 položiek, pri pokuse o spoluprácu s nimi sa môže zobraziť chyba prahovej hodnoty zobrazenia zoznamu.</span><span class="sxs-lookup"><span data-stu-id="5ded8-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="5ded8-104">Táto prahová hodnota sa uplatňuje na zachovanie výkonnosti služby.</span><span class="sxs-lookup"><span data-stu-id="5ded8-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="5ded8-105">Nemožno ju zmeniť.</span><span class="sxs-lookup"><span data-stu-id="5ded8-105">It can't be changed.</span></span> <span data-ttu-id="5ded8-106">Ak sa chcete vyhnúť zasiahnutiu tejto hranice:</span><span class="sxs-lookup"><span data-stu-id="5ded8-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="5ded8-107">**Používanie moderných**</span><span class="sxs-lookup"><span data-stu-id="5ded8-107">**Use modern**</span></span>

<span data-ttu-id="5ded8-108">Zobrazenia zobrazujúce veľa položiek fungujú najlepšie v modernom prostredí.</span><span class="sxs-lookup"><span data-stu-id="5ded8-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="5ded8-109">[Využite moderné prostredie](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , aby sa predišlo chybám, ktoré sa môžu zobraziť v klasickom prostredí.</span><span class="sxs-lookup"><span data-stu-id="5ded8-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="5ded8-110">**Pridanie indexov**</span><span class="sxs-lookup"><span data-stu-id="5ded8-110">**Add indexes**</span></span>

<span data-ttu-id="5ded8-111">Pri filtrovaní alebo zoraďovaní podľa stĺpca, ktorý nemá index, sa môže zobraziť chybové hlásenie.</span><span class="sxs-lookup"><span data-stu-id="5ded8-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="5ded8-112">Manuálne [Pridajte index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) z **nastavení zoznamu** v ponuke nastavenia a potom kliknite na položku **indexované stĺpce**.</span><span class="sxs-lookup"><span data-stu-id="5ded8-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="5ded8-113">**Úprava zobrazenia zoznamu**</span><span class="sxs-lookup"><span data-stu-id="5ded8-113">**Edit the list view**</span></span>

<span data-ttu-id="5ded8-114">Ak sa pri práci s veľkým zoznamom vyskytne chyba, [Upravte zobrazenie zoznamu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="5ded8-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="5ded8-115">Pri nasledujúcich štyroch zmenách sa odstránia prahové chyby zobrazenia zoznamu.</span><span class="sxs-lookup"><span data-stu-id="5ded8-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="5ded8-116">Vykonajte všetky štyri zmeny na odstránenie všetkých chýb.</span><span class="sxs-lookup"><span data-stu-id="5ded8-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="5ded8-117">Ak sa stále zobrazujú chyby, začiarknite políčko [spravovať veľké zoznamy a knižnice](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="5ded8-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="5ded8-118">Vyberte možnosť **žiadne** z **prvého zoradenia podľa stĺpca** a **potom položku Zoradiť podľa stĺpca**.</span><span class="sxs-lookup"><span data-stu-id="5ded8-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="5ded8-119">Vyberte možnosť **žiadne** z **prvej skupiny podľa stĺpca** a **potom položku Zoskupiť podľa stĺpca**.</span><span class="sxs-lookup"><span data-stu-id="5ded8-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="5ded8-120">Pre všetky stĺpce v časti **súčty** vyberte možnosť **žiadne** .</span><span class="sxs-lookup"><span data-stu-id="5ded8-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="5ded8-121">Zrušte začiarknutie políčka všetky, ale jeden stĺpec na zobrazenie v časti **stĺpce** .</span><span class="sxs-lookup"><span data-stu-id="5ded8-121">Deselect all but one column for display from the **Columns** section.</span></span>

