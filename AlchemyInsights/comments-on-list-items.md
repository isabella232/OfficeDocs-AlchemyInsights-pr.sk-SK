---
title: Komentáre k položkám zoznamu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982558"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="f174f-102">Komentáre k položkám zoznamu</span><span class="sxs-lookup"><span data-stu-id="f174f-102">Comments on List items</span></span>

<span data-ttu-id="f174f-103">Používatelia budú môcť čoskoro pridávať a odstraňovať komentáre k položkám zoznamu.</span><span class="sxs-lookup"><span data-stu-id="f174f-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="f174f-104">Používatelia môžu zobraziť všetky komentáre v položke zoznamu a filtrovať medzi zobrazeniami, ktoré zobrazujú komentáre alebo aktivitu súvisiacu s položkou.</span><span class="sxs-lookup"><span data-stu-id="f174f-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="f174f-105">**Časovanie** :</span><span class="sxs-lookup"><span data-stu-id="f174f-105">**Timing** :</span></span>

<span data-ttu-id="f174f-106">**Cielené vydanie** : postupné vydávanie v polovici októbra a očakáva sa, že sa ukončí v polovici novembra</span><span class="sxs-lookup"><span data-stu-id="f174f-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="f174f-107">**Standard Release** : postupné vydávanie v polovici novembra a očakávané ukončenie od začiatku decembra</span><span class="sxs-lookup"><span data-stu-id="f174f-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="f174f-108">**Zavádzanie** : cielené vydanie pre celú organizáciu</span><span class="sxs-lookup"><span data-stu-id="f174f-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="f174f-109">Používatelia musia pred pridaním a odstránením komentárov upozorniť na nasledujúce položky:</span><span class="sxs-lookup"><span data-stu-id="f174f-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="f174f-110">Komentáre dodržujte nastavenia povolení, ktoré sú vlastné v SharePointe.</span><span class="sxs-lookup"><span data-stu-id="f174f-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="f174f-111">Klasické zoznamy, ktoré ešte nie sú vytvorené tak, aby sa zobrazovali v moderných používateľských rozhraniach, ako sú napríklad zoznamy úloh, nebudú mať túto funkciu komentovania.</span><span class="sxs-lookup"><span data-stu-id="f174f-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="f174f-112">Komentovanie zoznamov v aplikácii teams nie je k dispozícii s týmto vydaním.</span><span class="sxs-lookup"><span data-stu-id="f174f-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="f174f-113">Komentáre nie sú indexované vyhľadávaním.</span><span class="sxs-lookup"><span data-stu-id="f174f-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="f174f-114">Správcovia môžu túto funkciu vypnúť na úrovni organizácie zmenou parametra **CommentsOnListItemsDisabled** v rutine typu cmdlet prostredia **Set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="f174f-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="f174f-115">V súčasnosti nie je možné zakázať komentovanie na úrovni lokality alebo zoznamu.</span><span class="sxs-lookup"><span data-stu-id="f174f-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="f174f-116">Dúfame, že tieto ovládacie prvky budú v neskoršej aktualizácii pravdepodobne v prvom štvrťroku 2021.</span><span class="sxs-lookup"><span data-stu-id="f174f-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
