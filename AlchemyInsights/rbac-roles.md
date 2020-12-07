---
title: 'Roly RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583952"
---
# <a name="rbac-rules"></a><span data-ttu-id="6a7fd-102">Pravidlá RBAC</span><span class="sxs-lookup"><span data-stu-id="6a7fd-102">RBAC rules</span></span>

<span data-ttu-id="6a7fd-103">Ak sa zobrazí chyba povolenia:</span><span class="sxs-lookup"><span data-stu-id="6a7fd-103">If you get the permission error:</span></span> 

- <span data-ttu-id="6a7fd-104">**Klient s identifikáciou objektu nemá povolenie na vykonávanie akcie nad rozsahom (kód: AuthorizationFailed)**: pri pokuse o vytvorenie zdroja Skontrolujte, či ste momentálne prihlásení pomocou používateľa, ktorému je priradená rola, ktorá má k zdroju povolenie zapisovať vo vybratom rozsahu.</span><span class="sxs-lookup"><span data-stu-id="6a7fd-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="6a7fd-105">Ak chcete napríklad spravovať virtuálne počítače v skupine zdrojov, mali by ste mať rolu [prispievateľa virtuálneho zariadenia](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) v skupine zdrojov (alebo nadradenom rozsahu).</span><span class="sxs-lookup"><span data-stu-id="6a7fd-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="6a7fd-106">Zoznam povolení pre každú vstavanú rolu nájdete [v téme vstavané roly Azure zdrojov](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6a7fd-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="6a7fd-107">**Nemáte povolenie na vytvorenie žiadosti o podporu**: pri pokuse o vytvorenie alebo aktualizáciu lístka technickej podpory Skontrolujte, či ste v súčasnosti prihlásení pomocou používateľa, ktorému je priradená rola s povolením Microsoft. support/supportTickets/write, ako je napríklad [prispievateľ žiadosti o podporu](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="6a7fd-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="6a7fd-108">**Nie je možné vytvoriť ďalšie priradenia rolí (kód: RoleAssignmentLimitExceeded)**: pri pokuse o priradenie roly skúste znížiť počet priradení rolí priradením rolí k skupinám.</span><span class="sxs-lookup"><span data-stu-id="6a7fd-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="6a7fd-109">Azure podporuje priradenia rolí až **2000** na predplatné.</span><span class="sxs-lookup"><span data-stu-id="6a7fd-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="6a7fd-110">Ďalšie informácie o rolách v službe Azure RBAC nájdete v téme roly v službe [Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6a7fd-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
