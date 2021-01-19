---
title: Riešenie problémov s vlastníkom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901278"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="c5cd4-102">Riešenie problémov s vlastníkom</span><span class="sxs-lookup"><span data-stu-id="c5cd4-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="c5cd4-103">Ak chcete riešiť problémy súvisiace s vlastníkom, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="c5cd4-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="c5cd4-104">[Pridanie alebo zmena správcov predplatného Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): skupiny Azure Active Directory (Azure AD) vlastní a spravuje vlastníci skupiny.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="c5cd4-105">Vlastníci skupiny môžu byť používatelia alebo princípy služieb a dokážu spravovať skupinu vrátane členstva.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="c5cd4-106">Vlastníci skupiny môžu priradiť len existujúcim vlastníkom skupiny alebo správcom skupiny.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="c5cd4-107">Vlastníci skupín nie sú povinní byť členmi skupiny.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="c5cd4-108">[Pridanie alebo zmena správcov predplatného Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): v tomto článku sa popisuje postup pridania alebo zmeny roly správcu pre používateľa pomocou služby Azure RBAC v rozsahu predplatného.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="c5cd4-109">Ak chcete pridať vlastníka skupiny alebo vlastníka aplikácie, použite prostredie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c5cd4-109">Use PowerShell to add a group owner or an application owner.</span></span>
