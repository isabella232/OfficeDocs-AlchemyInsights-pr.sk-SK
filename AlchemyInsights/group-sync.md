---
title: Synchronizácia skupiny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256918"
---
# <a name="group-sync"></a><span data-ttu-id="b5ba0-102">Synchronizácia skupiny</span><span class="sxs-lookup"><span data-stu-id="b5ba0-102">Group sync</span></span>

<span data-ttu-id="b5ba0-103">Tento článok obsahuje pokyny na synchronizáciu skupiny.</span><span class="sxs-lookup"><span data-stu-id="b5ba0-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="b5ba0-104">Ak globálny správca alebo vlastník skupiny nedokáže upraviť vlastnosti skupiny alebo pridať členov alebo priradiť vlastníkov na portáli Azure, uistite sa, že zdroj autority pre skupinu je Azure Active Directory (Azure AD) pre globálneho správcu alebo vlastníka skupiny na úpravu skupiny.</span><span class="sxs-lookup"><span data-stu-id="b5ba0-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="b5ba0-105">Pred pokusom o odstránenie synchronizovanej skupiny v službe Azure AD sa uistite, že ste [odstránili všetky priradené licencie](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) , aby sa predišlo chybám.</span><span class="sxs-lookup"><span data-stu-id="b5ba0-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="b5ba0-106">Informácie o synchronizácii používateľov, skupín a kontaktov nájdete v témach synchronizácia služby [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)a sledovanie [synchronizácie lokálnej skupiny na platforme Azure pomocou služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) na synchronizáciu lokálnych skupín pomocou funkcie ad Connect.</span><span class="sxs-lookup"><span data-stu-id="b5ba0-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="b5ba0-107">Pri riešení bežných chýb počas synchronizácie postupujte podľa tejto príručky [chyby pri riešení problémov počas synchronizácie](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) .</span><span class="sxs-lookup"><span data-stu-id="b5ba0-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

