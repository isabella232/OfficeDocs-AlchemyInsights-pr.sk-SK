---
title: Výkon problémy-SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719531"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8ed13-102">SharePoint alebo OneDrive pomalá, neprístupná alebo nedostupná pre viacerých používateľov</span><span class="sxs-lookup"><span data-stu-id="8ed13-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="8ed13-103">Ak lokalitu služby OneDrive alebo SharePoint nie je k dispozícii pre viacerých používateľov, ktorí predtým prístup, môže byť problém pri dočasnej služby.</span><span class="sxs-lookup"><span data-stu-id="8ed13-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8ed13-104">[Kontrola tabuľa stav služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8ed13-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="8ed13-105">Pridať a licencia používateľa</span><span class="sxs-lookup"><span data-stu-id="8ed13-105">Add and license the user</span></span>

<span data-ttu-id="8ed13-106">Zabezpečiť, že ste [priradiť licenciu na používateľov balíka Office 365 pre podniky](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="8ed13-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="8ed13-107">Priradenie povolení</span><span class="sxs-lookup"><span data-stu-id="8ed13-107">Assign Permissions</span></span>

<span data-ttu-id="8ed13-108">Ak používateľ nebola priradená licencia Sharepoint a stále sa zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či majú [príslušnú úroveň povolení](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) priradené.</span><span class="sxs-lookup"><span data-stu-id="8ed13-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="8ed13-109">Skúste použiť funkciu prístup žiadosť</span><span class="sxs-lookup"><span data-stu-id="8ed13-109">Consider using the access request feature</span></span>

<span data-ttu-id="8ed13-110">[Prístup žiadosť funkcia](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje ľuďom požiadať o prístup k obsahu, ktoré v súčasnosti nemajú povolenie na zobrazenie.</span><span class="sxs-lookup"><span data-stu-id="8ed13-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="8ed13-111">Povoliť vlastné skript môže spôsobiť prístup odmietnutý problémov</span><span class="sxs-lookup"><span data-stu-id="8ed13-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="8ed13-112">Existujú určité scenáre, kde funkciu *Povoliť vlastný skript* môže predkladať prístup odmietnutý.</span><span class="sxs-lookup"><span data-stu-id="8ed13-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="8ed13-113">Pre zoznam funkcií, ktoré sú postihnuté, zabezpečeniu a možnosť vypnúť funkciu.</span><span class="sxs-lookup"><span data-stu-id="8ed13-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8ed13-114">Prosím, navštívte [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8ed13-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

