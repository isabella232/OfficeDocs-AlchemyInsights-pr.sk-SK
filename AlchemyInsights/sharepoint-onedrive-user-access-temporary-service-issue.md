---
title: Problémy s výkonom-SharePoint alebo OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750571"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e27db-102">SharePoint alebo OneDrive pomalé, nedostupné alebo nedostupné pre viacerých používateľov</span><span class="sxs-lookup"><span data-stu-id="e27db-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="e27db-103">Ak OneDrive alebo lokality SharePoint nie je k dispozícii viacerým používateľom, ktorí predtým mali prístup, môže existovať dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="e27db-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="e27db-104">[Skontrolujte stav služby tabuľa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e27db-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="e27db-105">**Pridanie a licencia používateľa**</span><span class="sxs-lookup"><span data-stu-id="e27db-105">**Add and license the user**</span></span>

<span data-ttu-id="e27db-106">Uistite sa, že [priraďujete licencie používateľom balíka Office 365 pre podniky](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="e27db-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="e27db-107">**Priradiť povolenia**</span><span class="sxs-lookup"><span data-stu-id="e27db-107">**Assign Permissions**</span></span>

<span data-ttu-id="e27db-108">Ak používateľ bol priradený licenciu SharePoint a stále dostáva prístup odmietnutý správu, uistite sa, že majú [príslušné povolenie úroveň](https://docs.microsoft.com/sharepoint/understanding-permission-levels) priradená.</span><span class="sxs-lookup"><span data-stu-id="e27db-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="e27db-109">**Zvážte použitie funkcie žiadosti o prístup**</span><span class="sxs-lookup"><span data-stu-id="e27db-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="e27db-110">[Funkcia žiadosť o prístup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje ľuďom požiadať o prístup k obsahu, ktorý v súčasnosti nemajú povolenie na zobrazenie.</span><span class="sxs-lookup"><span data-stu-id="e27db-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="e27db-111">**Povoliť vlastný skript môže spôsobiť prístup odmietnutý problémy**</span><span class="sxs-lookup"><span data-stu-id="e27db-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="e27db-112">Existujú určité scenáre, kde *Povoliť vlastný skript* funkcia môže predstavovať prístup odmietnutý.</span><span class="sxs-lookup"><span data-stu-id="e27db-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="e27db-113">Zoznam ovplyvnených funkcií, bezpečnostných úvah a možnosti vypnutia funkcie.</span><span class="sxs-lookup"><span data-stu-id="e27db-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="e27db-114">Prosím, navštívte [Povoliť alebo zabrániť vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e27db-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

