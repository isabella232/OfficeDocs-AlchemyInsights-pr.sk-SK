---
title: Nasadenie doplnkov pre Aplikácie Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125685"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="fed0d-102">Nasadenie doplnkov pre Aplikácie Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fed0d-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="fed0d-103">Centralizované nasadenie je odporúčaným spôsobom nasadenia Office používateľom a skupinám vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="fed0d-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="fed0d-104">Ak chcete nasadiť doplnky, postupujte podľa nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="fed0d-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="fed0d-105">**Poznámka:** Ak chcete inštalovať doplnky pre Office ako jednotliví používateľ, pozrite si časť Zobrazenie, spravovanie a inštalácia doplnkov [Office programoch.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="fed0d-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="fed0d-106">Takisto sa uistite, že je Office povolený individuálne získavanie doplnkov z Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="fed0d-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="fed0d-107">Uistite sa, že vaše prostredie spĺňa požiadavky na nasadenie doplnkov pomocou funkcie Centralizované nasadenie.</span><span class="sxs-lookup"><span data-stu-id="fed0d-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="fed0d-108">Podrobnosti nájdete v téme [Požiadavky.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="fed0d-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="fed0d-109">Ak chcete **Nastavenia,** prejdite do časti Nastavenia Integrated Apps Get apps (Získať aplikácie s integrovanými aplikáciami) v centre spravovania služby  >    >   Microsoft 365 pre správcov.</span><span class="sxs-lookup"><span data-stu-id="fed0d-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="fed0d-110">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="fed0d-110">Notes:</span></span> 

- <span data-ttu-id="fed0d-111">Integrované aplikácie vyžadujú, aby správca získal povolenia globálneho správcu Exchange správcu.</span><span class="sxs-lookup"><span data-stu-id="fed0d-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="fed0d-112">Pri nasadzovaní doplnkov viacerým používateľom odporúčame priraďovanie pomocou skupín namiesto jednotlivých používateľov.</span><span class="sxs-lookup"><span data-stu-id="fed0d-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="fed0d-113">Podrobnosti nájdete v [téme Dôležité informácie pri priraďovaní doplnku používateľom a skupinám.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="fed0d-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="fed0d-114">Centralizované nasadenie nepodporuje používateľov vo vnorených skupinách ani skupinách, ktoré majú nadradené skupiny.</span><span class="sxs-lookup"><span data-stu-id="fed0d-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="fed0d-115">Podrobnosti nájdete v téme [Priradenia používateľov a skupín.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="fed0d-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="fed0d-116">Skontrolujte, či je služba správy aplikácií pre Microsoft 365 (GUID: 0517ffae-825d-4aff-999e-3f2336b8a20a) povolená pre používateľov na prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="fed0d-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="fed0d-117">Podrobnosti nájdete v téme [Konfigurácia vlastností aplikácie.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="fed0d-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="fed0d-118">Ak sa vyskytnú problémy s nasadením doplnkov pomocou funkcie Integrované aplikácie, skúste ich nasadiť [pomocou doplnkov.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="fed0d-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="fed0d-119">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="fed0d-119">For more information, see:</span></span>

<span data-ttu-id="fed0d-120">[Nasadenie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Spravovanie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Použitie rutín typu cmdlet prostredia PowerShell funkcie Centralizované](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) nasadenie na spravovanie doplnkov 
 [Publikovanie Office pomocou funkcie Centralizované nasadenie prostredníctvom Centra Microsoft 365 spravovania](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Riešenie problémov: Používateľovi sa doplnky nevidí](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Riešenie chýb používateľa Office inými doplnokmi](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="fed0d-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>