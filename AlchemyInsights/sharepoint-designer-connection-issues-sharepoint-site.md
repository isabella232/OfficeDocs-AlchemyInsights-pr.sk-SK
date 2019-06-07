---
title: Úrovne povolení v SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760707"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="2d22c-102">Problémy s pripojením programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="2d22c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="2d22c-103">Ak SharePoint Designer je problémy spojenie na lokality SharePoint, prosím, pokus o nasledujúce spoločné riešenia.</span><span class="sxs-lookup"><span data-stu-id="2d22c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="2d22c-104">Krok 1: Overte, či je aktualizovaný program SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="2d22c-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="2d22c-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="2d22c-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="2d22c-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="2d22c-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="2d22c-107">Aktualizácia pre program SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="2d22c-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="2d22c-108">Krok 2: Vymazať lokálne cache súbory</span><span class="sxs-lookup"><span data-stu-id="2d22c-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="2d22c-109">Zatvorte program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="2d22c-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="2d22c-110">Na lokálnom počítači, vyhľadajte nasledujúce priečinky odstrániť súbory vo vyrovnávacej pamäti.</span><span class="sxs-lookup"><span data-stu-id="2d22c-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="2d22c-111">Kliknite na tlačidlo Štart, spustiť a odstrániť všetky súbory nájdené v každej z nižšie umiestnenie.</span><span class="sxs-lookup"><span data-stu-id="2d22c-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="2d22c-112">%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="2d22c-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="2d22c-113">Otvorte program SharePoint Designer 2013 a zadajte konto znova, aby videli, či to funguje.</span><span class="sxs-lookup"><span data-stu-id="2d22c-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="2d22c-114">Krok 3: [umožniť moderné overenie Office 2013 v zariadení so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2d22c-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="2d22c-115">Krok 4: Správcovia musieť povoliť vlastné skript na povolenie pripojenia programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="2d22c-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="2d22c-116">Podrobný postup, príklady a úvah nájdete [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="2d22c-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


