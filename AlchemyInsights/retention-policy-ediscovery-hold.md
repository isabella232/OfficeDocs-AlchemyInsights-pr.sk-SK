---
title: 2609-zadržanie-alebo-eDiscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994094"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="e8104-102">Nie je možné odstrániť položky SharePoint Online alebo OneDrive pre podniky</span><span class="sxs-lookup"><span data-stu-id="e8104-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="e8104-103">Vy alebo vaši používatelia môžu byť schopní odstrániť položky SharePoint Online alebo OneDrive pre podniky, pretože politika uchovávania údajov, označenie uchovávania údajov alebo eDiscovery hold sa aplikuje na SharePoint OneDrive lokality alebo konkrétnu položku.</span><span class="sxs-lookup"><span data-stu-id="e8104-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="e8104-104">Toto zahŕňa možnosť odstránenia dokumentu, verzie dokumentu, priečinka, knižnice dokumentov, zoznamu, aplikácie, lokality alebo kolekcie lokalít.</span><span class="sxs-lookup"><span data-stu-id="e8104-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="e8104-105">Tu je niekoľko príkladov chybových hlásení, ktoré sa môžu prijímať pri pokuse o odstránenie položky, ktorá sa zachová:</span><span class="sxs-lookup"><span data-stu-id="e8104-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="e8104-106">"Táto stránka nemôže byť odstránená, pretože je zahrnutá v eDiscovery zadržanie alebo politiky uchovávania údajov"</span><span class="sxs-lookup"><span data-stu-id="e8104-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e8104-107">"Táto stránka má politiku súladu nastaviť blokovať odstránenie"</span><span class="sxs-lookup"><span data-stu-id="e8104-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="e8104-108">"Politika súladu je v súčasnosti blokuje odstránenie tejto lokality"</span><span class="sxs-lookup"><span data-stu-id="e8104-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="e8104-109">"Táto kolekcia lokalít nie je možné odstrániť, pretože obsahuje lokality, ktoré sú súčasťou eDiscovery zadržanie alebo politiky uchovávania údajov"</span><span class="sxs-lookup"><span data-stu-id="e8104-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e8104-110">"Musíte odstrániť všetky položky v tomto priečinku pred odstránením priečinka"</span><span class="sxs-lookup"><span data-stu-id="e8104-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="e8104-111">"Verzie tejto položky nie je možné odstrániť, pretože je v zadržanie alebo politika uchovávania údajov"</span><span class="sxs-lookup"><span data-stu-id="e8104-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="e8104-112">"Položka sa nedá odstrániť počas podržania"</span><span class="sxs-lookup"><span data-stu-id="e8104-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="e8104-113">"Štítok, ktorý sa aplikuje na túto položku zabraňuje jeho úprave alebo odstráneniu"</span><span class="sxs-lookup"><span data-stu-id="e8104-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="e8104-114">"Zoznam nie je možné odstrániť pri podržaní alebo uchovávania politiky"</span><span class="sxs-lookup"><span data-stu-id="e8104-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="e8104-115">"Zoznam nie je možné odstrániť, ak je blokovaný alebo ak politika uchovávania údajov je použitá na to"</span><span class="sxs-lookup"><span data-stu-id="e8104-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="e8104-116">Ak chcete odstrániť položky v jednom z týchto scenárov, musí sa odstrániť politika uchovávania údajov, štítok uchovávania údajov alebo zadržanie eDiscovery (alebo lokalita musí byť vylúčená z politiky uchovávania údajov).</span><span class="sxs-lookup"><span data-stu-id="e8104-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="e8104-117">Musíte buď vypnúť alebo vylúčiť príslušné držanie, ktoré spôsobuje tento problém.</span><span class="sxs-lookup"><span data-stu-id="e8104-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e8104-118">Po odstránení politiky uchovávania alebo zadržania môže zmena trvať až 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="e8104-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="e8104-119">Ďalšie informácie o rôznych funkciách uchovávania a zadržania, ktoré možno aplikovať na lokality SharePoint a kontá OneDrive, nájdete v niektorej z nasledujúcich tém.</span><span class="sxs-lookup"><span data-stu-id="e8104-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="e8104-120">Prehľad politík uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="e8104-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="e8104-121">Prehľad štítkov uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="e8104-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="e8104-122">Správa drží v pokročilom eDiscovery</span><span class="sxs-lookup"><span data-stu-id="e8104-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="e8104-123">eDiscovery drží</span><span class="sxs-lookup"><span data-stu-id="e8104-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="e8104-124">Staršie politiky uzavretia a odstránenia lokality</span><span class="sxs-lookup"><span data-stu-id="e8104-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
