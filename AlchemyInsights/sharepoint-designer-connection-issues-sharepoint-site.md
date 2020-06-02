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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511559"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b252c-102">Problémy s pripojením programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b252c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b252c-103">Ak sa v programe SharePoint Designer vyskytli problémy s pripojením na lokality SharePoint, vyskúšajte nasledujúce bežné riešenia.</span><span class="sxs-lookup"><span data-stu-id="b252c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="b252c-104">Krok 1: Overte, či je program SharePoint Designer 2013 aktualizovaný [sharepointovým balíkom Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a aktualizáciou programu [SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)2.</span><span class="sxs-lookup"><span data-stu-id="b252c-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="b252c-105">Krok 2: Vymažte lokálne súbory vyrovnávacej pamäte:</span><span class="sxs-lookup"><span data-stu-id="b252c-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="b252c-106">Zatvorte program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b252c-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="b252c-107">Na lokálnom počítači odstráňte všetky súbory nájdené v každom z nasledujúcich priečinkov.</span><span class="sxs-lookup"><span data-stu-id="b252c-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="b252c-108">%APPDATA%\Microsoft\Rozšírenia webového servera\Vyrovnávacia pamäť</span><span class="sxs-lookup"><span data-stu-id="b252c-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="b252c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="b252c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="b252c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b252c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="b252c-111">Otvorte SharePoint Designer 2013 a znova zadajte konto, aby ste zistili, či funguje.</span><span class="sxs-lookup"><span data-stu-id="b252c-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b252c-112">Krok 3: [Povolenie moderného overovania balíka Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b252c-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="b252c-113">Krok 4: Správcovia budú musieť **povoliť vlastný skript** v nastaveniach Centra spravovania služby SharePoint, aby bolo možné pripojenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b252c-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="b252c-114">Ďalšie informácie nájdete v téme [Povolenie alebo zakázanie vlastného skriptu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="b252c-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


