---
title: Problémy s výkonom – SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771259"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="41070-102">Služby SharePoint alebo OneDrive sú pomalé, nedostupné alebo nie sú k dispozícii pre viacerých používateľov</span><span class="sxs-lookup"><span data-stu-id="41070-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="41070-103">Ak OneDrive alebo SharePoint nie je k dispozícii viacerým používateľom, ktorí mali predtým prístup, môže sa vyskytnúť dočasný problém so službou.</span><span class="sxs-lookup"><span data-stu-id="41070-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="41070-104">[Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="41070-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="41070-105">**Pridanie a povolenie používateľa**</span><span class="sxs-lookup"><span data-stu-id="41070-105">**Add and license the user**</span></span>

<span data-ttu-id="41070-106">Uistite sa, že [priraďujete licencie používateľom v službe Microsoft 365 for Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="41070-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="41070-107">**Priradenie povolení**</span><span class="sxs-lookup"><span data-stu-id="41070-107">**Assign Permissions**</span></span>

<span data-ttu-id="41070-108">Ak je používateľovi priradená licencia na SharePoint a stále sa zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či majú priradenú [zodpovedajúcu úroveň povolení](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="41070-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="41070-109">**Zvážte použitie funkcie žiadosť o prístup**</span><span class="sxs-lookup"><span data-stu-id="41070-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="41070-110">[Funkcia žiadosti o prístup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje ľuďom požiadať o prístup k obsahu, ktorý momentálne nemajú povolenie na zobrazenie.</span><span class="sxs-lookup"><span data-stu-id="41070-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="41070-111">**Povolenie vlastného skriptu môže spôsobiť problémy s prístupom k odmietnutým**</span><span class="sxs-lookup"><span data-stu-id="41070-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="41070-112">K dispozícii sú určité scenáre, v ktorých môže funkcia *Povoliť vlastný skript* prezentovať prístup odmietnutý.</span><span class="sxs-lookup"><span data-stu-id="41070-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="41070-113">Zoznam ovplyvnených funkcií, dôvody zabezpečenia a možnosť vypnutia funkcie.</span><span class="sxs-lookup"><span data-stu-id="41070-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="41070-114">Prejdite na stránku [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="41070-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

