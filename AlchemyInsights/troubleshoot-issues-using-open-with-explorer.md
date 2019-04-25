---
title: Riešenie problémov pomocou Open Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390622"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="e2f68-102">Riešenie problémov s Open s Explorer</span><span class="sxs-lookup"><span data-stu-id="e2f68-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="e2f68-103">Vyriešiť bežné problémy s otváraním knižnica dokumentov SharePoint alebo OneDrive pomocou príkazu **Otvoriť v programe Prieskumník** :</span><span class="sxs-lookup"><span data-stu-id="e2f68-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="e2f68-104">Pomocou programu Internet Explorer 10 alebo Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="e2f68-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="e2f68-105">**Otvoriť v programe Prieskumník** nie je kompatibilný s Microsoft Edge, prehliadač Google Chrome, Firefox a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="e2f68-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e2f68-106">**Open s Explorer** vypnutá vo všetkých prehliadačoch okrem programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e2f68-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="e2f68-107">**Otvoriť v programe Prieskumník** nie je k dispozícii v modernej skúsenosti pre knižnice.</span><span class="sxs-lookup"><span data-stu-id="e2f68-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="e2f68-108">Použite **zobrazenie v Prieskumníkovi** .</span><span class="sxs-lookup"><span data-stu-id="e2f68-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="e2f68-109">Vyberte **Zobraziť možnosti** \> **zobrazenie v Prieskumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="e2f68-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="e2f68-110">Zobrazenie v Prieskumníkovi súborov nie je kompatibilný s Microsoft Edge, prehliadač Google Chrome, Firefox a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="e2f68-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e2f68-111">**Zobrazenie v Prieskumníkovi súborov** k dispozícii len v programe Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e2f68-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="e2f68-112">Uistite sa, že je spustená služba WebClient.</span><span class="sxs-lookup"><span data-stu-id="e2f68-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="e2f68-113">Do poľa Hľadať systém Windows zadajte spustiť, vyberte počítačovú aplikáciu spustiť, zadajte services.msc a stlačte kláves Enter.</span><span class="sxs-lookup"><span data-stu-id="e2f68-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="e2f68-114">Prejdite na službu WebClient a skontrolujte **stav** stĺpec zobrazí "Beží."</span><span class="sxs-lookup"><span data-stu-id="e2f68-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="e2f68-115">Ak nie, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="e2f68-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e2f68-116">(Musíte najprv zapnúť službu výberom buď **manuálne** alebo **automaticky** v **Typ spustenia** políčka.)</span><span class="sxs-lookup"><span data-stu-id="e2f68-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e2f68-117">Otvorenie knižnice v programe Prieskumník sa hodí, ak potrebujete na kopírovanie alebo presúvanie viacerých súborov a priečinkov, akonáhle, ale ak chcete pravidelne pracovať v knižnici, odporúčame vám jeho synchronizáciu.</span><span class="sxs-lookup"><span data-stu-id="e2f68-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="e2f68-118">Riešenie problémov otvoriť v programe Prieskumník, pozrite si [Otvoriť v programe Prieskumník](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e2f68-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e2f68-119">Informácie o nastavení synchronizácie, pozrite si [synchronizovať SharePoint súbory pomocou nového klienta synchronizácie OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e2f68-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="e2f68-120">Prečítajte si článok [ako používať príkaz "Open s Explorer" riešenie problémov v službe SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="e2f68-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

