---
title: V programe Outlook sa nezobrazujú doplnky pre jedného používateľa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198219"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="e834d-102">V programe Outlook sa nezobrazujú doplnky pre jedného používateľa</span><span class="sxs-lookup"><span data-stu-id="e834d-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="e834d-103">Používateľ môže byť súčasťou roly, ktorá nemá správny parameter AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="e834d-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="e834d-104">Spustite tento cmdlet zistiť, či je k používateľovi priradená správna rola:</span><span class="sxs-lookup"><span data-stu-id="e834d-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="e834d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegovanie $false | Formát-tabuľka -automatická úloha,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="e834d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="e834d-106">Ďalšie informácie nájdete v téme [Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e834d-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
