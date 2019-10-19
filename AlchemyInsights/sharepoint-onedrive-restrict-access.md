---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750679"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d4484-102">Obmedzenie prístupu v SharePointe alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="d4484-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d4484-103">Existuje mnoho spôsobov, ako obmedziť prístup k službám SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4484-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="d4484-104">Tieto rôzne metódy obmedzenia prístupu sú uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="d4484-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="d4484-105">**Obmedzenie povolení**</span><span class="sxs-lookup"><span data-stu-id="d4484-105">**Permission Restriction**</span></span>

<span data-ttu-id="d4484-106">V službe SharePoint Online a OneDrive for Business Obmedzujeme prístup k položkám, ako sú lokality, súbory a priečinky, a to iba poskytnutím prístupu k tým skupinám/jednotlivcom, ktorí majú prístup.</span><span class="sxs-lookup"><span data-stu-id="d4484-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="d4484-107">Prispôsobenie povolení pre zoznam alebo knižnicu lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="d4484-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="d4484-108">Prispôsobenie povolení lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="d4484-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="d4484-109">Zmena povolení pre podpriečinok</span><span class="sxs-lookup"><span data-stu-id="d4484-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="d4484-110">Ovládanie prístupu z nespravovaných zariadení</span><span class="sxs-lookup"><span data-stu-id="d4484-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="d4484-111">Ako SharePoint alebo globálny admin v balíku Office 365, môžete blokovať alebo obmedziť prístup k SharePoint a OneDrive obsah z nespravované zariadenia (tie nie hybridné AD pripojil alebo kompatibilné s Intune).</span><span class="sxs-lookup"><span data-stu-id="d4484-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="d4484-112">**Obmedzenie sieťového umiestnenia**</span><span class="sxs-lookup"><span data-stu-id="d4484-112">**Network Location Restriction**</span></span>

<span data-ttu-id="d4484-113">Ako správca IT môžete ovládať prístup k prostriedkom služby SharePoint a OneDrive na základe definovaných sieťových umiestnení, ktorým dôverujete.</span><span class="sxs-lookup"><span data-stu-id="d4484-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="d4484-114">Toto je známe aj ako politika založená na polohe.</span><span class="sxs-lookup"><span data-stu-id="d4484-114">This is also known as location-based policy.</span></span> <span data-ttu-id="d4484-115">Ďalšie informácie nájdete [v téme kontrola prístupu k údajom služby SharePoint Online a OneDrive na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="d4484-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="d4484-116">**Obmedzenie zámku lokality**</span><span class="sxs-lookup"><span data-stu-id="d4484-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="d4484-117">V rámci služby SharePoint Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup.</span><span class="sxs-lookup"><span data-stu-id="d4484-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="d4484-118">Toto je nastavené pomocou prostredia PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosť [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="d4484-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="d4484-119">**Obmedzenie používateľov na vytváranie lokalít alebo podlokalít**</span><span class="sxs-lookup"><span data-stu-id="d4484-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="d4484-120">Ako správca lokality SharePoint alebo Office 365 globálny správca, môžete umožniť používateľom vytvárať a spravovať svoje vlastné lokality SharePoint, určiť, aký druh lokalít, ktoré môžu vytvoriť, a určiť umiestnenie lokalít.</span><span class="sxs-lookup"><span data-stu-id="d4484-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="d4484-121">Ďalšie informácie nájdete [v téme Spravovanie vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d4484-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

