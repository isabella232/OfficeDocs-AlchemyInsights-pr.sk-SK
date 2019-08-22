---
title: Obmedzenie prístupu v SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559892"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="91d07-102">Obmedzenie prístupu v SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="91d07-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="91d07-103">Existuje mnoho spôsobov, ako obmedziť prístup k SharePoint Online/OneDrive služby.</span><span class="sxs-lookup"><span data-stu-id="91d07-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="91d07-104">Tieto rôzne metódy obmedzenie prístupu sú uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="91d07-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="91d07-105">**Povolenie obmedzenie**</span><span class="sxs-lookup"><span data-stu-id="91d07-105">**Permission Restriction**</span></span>

<span data-ttu-id="91d07-106">SharePoint Online a OneDrive pre podniky, Obmedzujeme prístup položiek lokality, súbory a priečinky, ako iba poskytnutím prístupu pre tie skupiny/jednotlivcov, ktorí by mali mať prístup.</span><span class="sxs-lookup"><span data-stu-id="91d07-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="91d07-107">Prispôsobiť povolenia pre zoznam SharePoint alebo knižnicu</span><span class="sxs-lookup"><span data-stu-id="91d07-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="91d07-108">Prispôsobiť povolenia pre lokalitu SharePoint</span><span class="sxs-lookup"><span data-stu-id="91d07-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="91d07-109">Zmeniť povolenia na podpriečinok</span><span class="sxs-lookup"><span data-stu-id="91d07-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="91d07-110">Kontrola prístupu z nespravovaná zariadení</span><span class="sxs-lookup"><span data-stu-id="91d07-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="91d07-111">Ako SharePoint alebo Office 365 globálne admin, môžete zablokovať alebo obmedziť prístup k obsahu služby SharePoint a OneDrive z nespravovaná zariadení (tie hybridné AD pripojil alebo kompatibilné s Windows Intune).</span><span class="sxs-lookup"><span data-stu-id="91d07-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="91d07-112">**Sieťové umiestnenie obmedzenia**</span><span class="sxs-lookup"><span data-stu-id="91d07-112">**Network Location Restriction**</span></span>

<span data-ttu-id="91d07-113">Ako správca IT, môžete ovládať prístup k službe SharePoint a OneDrive zdrojov na základe definovaných sieťových umiestneniach, ktoré dôverujete.</span><span class="sxs-lookup"><span data-stu-id="91d07-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="91d07-114">To je tiež známy ako umiestnenie-založené politiky.</span><span class="sxs-lookup"><span data-stu-id="91d07-114">This is also known as location-based policy.</span></span> <span data-ttu-id="91d07-115">Pre viac informácií, prečítajte si [Kontrola prístupu k SharePoint Online a OneDrive údajov na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="91d07-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="91d07-116">**Obmedzenie lokality zámok**</span><span class="sxs-lookup"><span data-stu-id="91d07-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="91d07-117">V rámci SharePoint Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup.</span><span class="sxs-lookup"><span data-stu-id="91d07-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="91d07-118">Toto sa nastaví pomocou PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosť uzamknutia - [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="91d07-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="91d07-119">**Obmedziť používateľov od vytvorenia lokalít alebo podlokality**</span><span class="sxs-lookup"><span data-stu-id="91d07-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="91d07-120">Ako SharePoint admin alebo Office 365 globálne admin, umožníte používateľom vytvoriť a spravovať vlastné lokality SharePoint, určiť, aký druh stránok môžu vytvárať, a zadajte umiestnenie lokalít.</span><span class="sxs-lookup"><span data-stu-id="91d07-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="91d07-121">Pre viac informácií, prečítajte si [Vytvorenie spravovať lokality SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="91d07-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

