---
title: Problémy s pripojením programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051728"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c4fa4-102">Problémy s pripojením programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="c4fa4-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c4fa4-103">Ak SharePoint Designer zažíva problémy s pripojením na lokality SharePoint, vyskúšajte nasledujúce bežné riešenia.</span><span class="sxs-lookup"><span data-stu-id="c4fa4-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="c4fa4-104">Krok 1: Skontrolujte, či SharePoint Designer 2013 sa aktualizuje [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [August 2, 2016 aktualizácie programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="c4fa4-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="c4fa4-105">Krok 2: Vymažte lokálne súbory vyrovnávacej pamäte:</span><span class="sxs-lookup"><span data-stu-id="c4fa4-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="c4fa4-106">Zatvorte program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c4fa4-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="c4fa4-107">V lokálnom počítači odstráňte všetky súbory nájdené v každom z nasledujúcich priečinkov.</span><span class="sxs-lookup"><span data-stu-id="c4fa4-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="c4fa4-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="c4fa4-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="c4fa4-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="c4fa4-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="c4fa4-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="c4fa4-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="c4fa4-111">Otvorte SharePoint Designer 2013 a zadajte konto znova, aby zistil, či to funguje.</span><span class="sxs-lookup"><span data-stu-id="c4fa4-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c4fa4-112">Krok 3: [Povoliť moderné overovanie pre balík Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c4fa4-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="c4fa4-113">Krok 4: Správcovia budú musieť **Povoliť vlastný skript** v nastavení služby SharePoint admin Center povoliť pripojenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="c4fa4-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="c4fa4-114">Ďalšie informácie nájdete v téme [povolenie alebo predchádzanie vlastným skriptom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="c4fa4-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


