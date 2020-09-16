---
title: Problémy s pripojením v programe SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727186"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="a6d4e-102">Problémy s pripojením v programe SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="a6d4e-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="a6d4e-103">Ak SharePoint Designer zažíva problémy s pripojením na lokality SharePoint, vyskúšajte tieto bežné riešenia.</span><span class="sxs-lookup"><span data-stu-id="a6d4e-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="a6d4e-104">Krok 1: overenie, či sa SharePoint Designer 2013 aktualizuje pomocou [služby SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [aktualizácie z augusta 2, 2016 pre SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="a6d4e-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="a6d4e-105">Krok 2: Vymazanie lokálnych súborov vyrovnávacej pamäte:</span><span class="sxs-lookup"><span data-stu-id="a6d4e-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="a6d4e-106">Zatvorenie programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a6d4e-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="a6d4e-107">V lokálnom počítači odstráňte všetky súbory nájdené v každom z týchto priečinkov.</span><span class="sxs-lookup"><span data-stu-id="a6d4e-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="a6d4e-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="a6d4e-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="a6d4e-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="a6d4e-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="a6d4e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="a6d4e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="a6d4e-111">Otvorte SharePoint Designer 2013 a znova zadajte konto, aby ste zistili, či to funguje.</span><span class="sxs-lookup"><span data-stu-id="a6d4e-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="a6d4e-112">Krok 3: [povolenie moderného overovania pre Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a6d4e-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="a6d4e-113">Krok 4: Správcovia budú musieť **Povoliť vlastné skripty** v nastaveniach centra spravovania služby SharePoint, aby sa umožnilo pripojenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="a6d4e-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="a6d4e-114">Ďalšie informácie nájdete v téme [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="a6d4e-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


