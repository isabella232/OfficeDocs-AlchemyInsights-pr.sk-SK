---
title: 2609 – retenčné-alebo-eDiscovery
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727906"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="dd4c8-102">Nie je možné odstrániť položky v SharePointe Online alebo vo OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="dd4c8-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="dd4c8-103">Vy alebo vaši používatelia nie je možné odstrániť položky v SharePointe Online alebo vo OneDrive for Business, pretože politika uchovávania údajov, označenie uchovávania údajov alebo zadržanie eDiscovery sa použijú na lokalitu SharePoint na lokalite OneDrive alebo na konkrétnu položku.</span><span class="sxs-lookup"><span data-stu-id="dd4c8-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="dd4c8-104">Toto zahŕňa neschopnosť odstrániť dokument, verziu dokumentu, priečinok, knižnicu dokumentov, zoznam, aplikáciu, lokalitu alebo kolekciu lokalít.</span><span class="sxs-lookup"><span data-stu-id="dd4c8-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="dd4c8-105">Ak chcete odstrániť položky v niektorom z týchto scenárov, musí sa odstrániť politika uchovávania údajov, označenie uchovávania údajov alebo zadržanie eDiscovery (alebo lokalita musí byť vyňatá z politiky uchovávania údajov).</span><span class="sxs-lookup"><span data-stu-id="dd4c8-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="dd4c8-106">Je potrebné vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém.</span><span class="sxs-lookup"><span data-stu-id="dd4c8-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="dd4c8-107">Po odstránení politiky alebo zadržania uchovávania údajov môže zmena nadobudnúť až 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="dd4c8-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="dd4c8-108">Ďalšie informácie o rôznych funkciách uchovávania a držania, ktoré možno použiť na lokalitách SharePoint a kontách OneDrive, nájdete v niektorej z týchto tém:</span><span class="sxs-lookup"><span data-stu-id="dd4c8-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="dd4c8-109">Prehľad politík uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="dd4c8-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="dd4c8-110">Prehľad označení uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="dd4c8-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="dd4c8-111">Správa zadržaní v rozšírených Ediscoverách</span><span class="sxs-lookup"><span data-stu-id="dd4c8-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="dd4c8-112">uchovávanie eDiscovery</span><span class="sxs-lookup"><span data-stu-id="dd4c8-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="dd4c8-113">Politiky ukončenia a odstraňovania starších lokalít</span><span class="sxs-lookup"><span data-stu-id="dd4c8-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)