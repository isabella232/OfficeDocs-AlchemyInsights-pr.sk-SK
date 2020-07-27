---
title: Viacerí používatelia získajú chybu prístup odmietnutý pri pridávaní doplnkov v programe Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424174"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="7019d-102">Viacerí používatelia získajú chybu prístup odmietnutý pri pridávaní doplnkov v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="7019d-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="7019d-103">Môžete určiť, ktorí správcovia vo vašej organizácii majú povolenia na inštaláciu a správu doplnkov pre program Outlook.</span><span class="sxs-lookup"><span data-stu-id="7019d-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="7019d-104">Môžete tiež určiť, ktorí používatelia vo vašej organizácii majú povolenie na inštaláciu a správu doplnkov pre vlastné použitie.</span><span class="sxs-lookup"><span data-stu-id="7019d-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="7019d-105">Podrobnosti nájdete v [téme Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="7019d-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="7019d-106">Ak chcete overiť, či ste úspešne priradili povolenia pre používateľa, nahraďte názov roly na overenie a spustite nasledujúci príkaz v <Role Name> prostredí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7019d-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="7019d-107">Získajte ManagementRoleAssignment -Úloha " <Role Name> " - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="7019d-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="7019d-108">V tomto príklade sa uvádza, ako overiť, komu ste priradili povolenia na inštaláciu doplnkov z Office Obchodu pre organizáciu.</span><span class="sxs-lookup"><span data-stu-id="7019d-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="7019d-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="7019d-109">PowerShell</span></span>

<span data-ttu-id="7019d-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="7019d-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="7019d-111">Vo výsledkoch Get-ManagementRoleAssignment, skontrolujte položky v stĺpci Efektívni používatelia.</span><span class="sxs-lookup"><span data-stu-id="7019d-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="7019d-112">Podrobné informácie o syntaxi a parametroch nájdete [v téme Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="7019d-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 