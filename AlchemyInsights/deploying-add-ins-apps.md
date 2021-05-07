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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233549"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="d9db1-102">Nasadenie doplnkov pre Aplikácie Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d9db1-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="d9db1-103">Centralizované nasadenie je odporúčaným spôsobom nasadenia Office používateľom a skupinám vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="d9db1-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="d9db1-104">Ak chcete nasadiť doplnky, postupujte podľa nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="d9db1-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="d9db1-105">**Poznámka:** Ak chcete inštalovať doplnky pre Office ako jednotliví používateľ, pozrite si časť Zobrazenie, spravovanie a inštalácia doplnkov [Office programoch.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="d9db1-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="d9db1-106">Takisto sa uistite, že je Office povolený individuálne získavanie doplnkov z Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="d9db1-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="d9db1-107">Podrobnosti nájdete v téme Zabránenie sťahovaniu doplnkov vypnutím služby Office Store vo všetkých [klientoch (okrem Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="d9db1-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="d9db1-108">Uistite sa, že vaše prostredie spĺňa požiadavky na nasadenie doplnkov pomocou funkcie Centralizované nasadenie.</span><span class="sxs-lookup"><span data-stu-id="d9db1-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="d9db1-109">Podrobnosti nájdete v téme [Požiadavky.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="d9db1-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="d9db1-110">Ak chcete **Nastavenia,** prejdite do časti Nastavenia Integrated Apps Get apps (Získať aplikácie s integrovanými aplikáciami) v centre spravovania služby  >    >   Microsoft 365 pre správcov.</span><span class="sxs-lookup"><span data-stu-id="d9db1-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="d9db1-111">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="d9db1-111">Notes:</span></span> 

- <span data-ttu-id="d9db1-112">Integrované aplikácie vyžadujú, aby správca získal povolenia globálneho správcu Exchange správcu.</span><span class="sxs-lookup"><span data-stu-id="d9db1-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="d9db1-113">Pri nasadzovaní doplnkov viacerým používateľom odporúčame priraďovanie pomocou skupín namiesto jednotlivých používateľov.</span><span class="sxs-lookup"><span data-stu-id="d9db1-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="d9db1-114">Podrobnosti nájdete v [téme Dôležité informácie pri priraďovaní doplnku používateľom a skupinám.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="d9db1-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="d9db1-115">Centralizované nasadenie nepodporuje používateľov vo vnorených skupinách ani skupinách, ktoré majú nadradené skupiny.</span><span class="sxs-lookup"><span data-stu-id="d9db1-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="d9db1-116">Podrobnosti nájdete v téme [Priradenia používateľov a skupín.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="d9db1-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="d9db1-117">Skontrolujte, či je služba správy aplikácií pre Microsoft 365 (GUID: 0517ffae-825d-4aff-999e-3f2336b8a20a) povolená pre používateľov na prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="d9db1-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="d9db1-118">Podrobnosti nájdete v téme [Konfigurácia vlastností aplikácie.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="d9db1-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="d9db1-119">Ak sa vyskytnú problémy s nasadením doplnkov pomocou funkcie Integrované aplikácie, skúste ich nasadiť [pomocou doplnkov.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="d9db1-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="d9db1-120">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="d9db1-120">For more information, see:</span></span>

<span data-ttu-id="d9db1-121">[Nasadenie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Spravovanie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Použitie rutín typu cmdlet prostredia PowerShell funkcie Centralizované](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) nasadenie na spravovanie doplnkov 
 [Publikovanie Office pomocou funkcie Centralizované nasadenie prostredníctvom Centra Microsoft 365 spravovania](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Riešenie problémov: Používateľovi sa doplnky nevidí](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Riešenie chýb používateľa Office inými doplnokmi](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="d9db1-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>