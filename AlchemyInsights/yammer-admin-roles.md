---
title: Informácie o správcovi siete Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038124"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="ce204-102">Informácie o správcovi siete Yammer</span><span class="sxs-lookup"><span data-stu-id="ce204-102">About Yammer admins</span></span>

<span data-ttu-id="ce204-103">**Správcovia siete**</span><span class="sxs-lookup"><span data-stu-id="ce204-103">**Network admins**</span></span>

<span data-ttu-id="ce204-104">Globálni správcovia sa automaticky povýšený na overené roly správcu v sieti Yammer.</span><span class="sxs-lookup"><span data-stu-id="ce204-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="ce204-105">V nasledujúcich prípadoch sa táto propagácia nemusí správne vyskytnúť:</span><span class="sxs-lookup"><span data-stu-id="ce204-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="ce204-106">Existujú viaceré siete Yammeru a správca sa prihlási do nesprávneho.</span><span class="sxs-lookup"><span data-stu-id="ce204-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="ce204-107">Na prístup k jednej sieti Yammeru sa vyžaduje [zlúčenie siete](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) .</span><span class="sxs-lookup"><span data-stu-id="ce204-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="ce204-108">Používa sa Azure PIM.</span><span class="sxs-lookup"><span data-stu-id="ce204-108">Azure PIM is being used.</span></span> <span data-ttu-id="ce204-109">Používateľ sa nemusí povýšiť na globálneho správcu dostatočne dlho na to, aby sa táto propagačná akcia mohla vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="ce204-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="ce204-110">Budúce aktualizácie na Yammer môže vyriešiť tento problém, ale je najlepšie podporiť používateľov globálneho správcu manuálne.</span><span class="sxs-lookup"><span data-stu-id="ce204-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="ce204-111">Problém so synchronizáciou existuje v sieti Yammer.</span><span class="sxs-lookup"><span data-stu-id="ce204-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="ce204-112">V tomto prípade sa vyžaduje žiadosť o podporu na ďalšie šetrenie.</span><span class="sxs-lookup"><span data-stu-id="ce204-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="ce204-113">Ďalšie informácie o rolách správcu Yammera nájdete v téme [Správa správcov yammera](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="ce204-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="ce204-114">**Správcovia skupiny**</span><span class="sxs-lookup"><span data-stu-id="ce204-114">**Group admins**</span></span>

<span data-ttu-id="ce204-115">Správcovia skupiny pre služby Microsoft 365 pripojené skupiny sa synchronizujú s členstvom v skupine z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce204-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="ce204-116">Pre veľké skupiny môže táto synchronizácia trvať dlhšiu dobu.</span><span class="sxs-lookup"><span data-stu-id="ce204-116">For large groups, this sync can take an extended period.</span></span>
