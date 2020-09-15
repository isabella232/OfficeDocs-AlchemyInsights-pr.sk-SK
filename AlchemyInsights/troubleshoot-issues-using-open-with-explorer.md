---
title: Riešenie problémov s použitím funkcie otvoriť v programe Prieskumník
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659073"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="4edc2-102">Riešenie problémov s otvorením v programe Prieskumník</span><span class="sxs-lookup"><span data-stu-id="4edc2-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="4edc2-103">Riešenie bežných problémov s otvorením knižnice dokumentov v SharePointe alebo vo OneDrive pomocou príkazu **Otvoriť v programe Prieskumník** :</span><span class="sxs-lookup"><span data-stu-id="4edc2-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="4edc2-104">Použite Internet Explorer 10 alebo Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="4edc2-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="4edc2-105">**Otvoriť v programe Prieskumník** nie je kompatibilný s prehliadačom Microsoft Edge, Google Chrome, Firefox a ďalšími používateľmi.</span><span class="sxs-lookup"><span data-stu-id="4edc2-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="4edc2-106">**Otvoriť v programe Prieskumník** je vo všetkých prehliadačoch zakázaný okrem programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="4edc2-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="4edc2-107">**Otvoriť v programe Prieskumník** nie je k dispozícii v modernom prostredí knižníc SharePointu.</span><span class="sxs-lookup"><span data-stu-id="4edc2-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="4edc2-108">Namiesto toho použite **zobrazenie v Prieskumníkovi** .</span><span class="sxs-lookup"><span data-stu-id="4edc2-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="4edc2-109">Vyberte zobrazenie **Možnosti zobrazenia** \> **v Prieskumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="4edc2-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="4edc2-110">Zobrazenie v Prieskumníkovi nie je kompatibilné s prehliadačom Microsoft Edge, Google Chrome, Firefoxom a ďalšími používateľmi.</span><span class="sxs-lookup"><span data-stu-id="4edc2-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="4edc2-111">**Zobrazenie v Prieskumníkovi** je k dispozícii len v Internet Exploreri.</span><span class="sxs-lookup"><span data-stu-id="4edc2-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="4edc2-112">Skontrolujte, či je spustená služba WebClient.</span><span class="sxs-lookup"><span data-stu-id="4edc2-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="4edc2-113">Do poľa Windows Search zadajte text spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte výraz Services. msc a potom stlačte kláves ENTER.</span><span class="sxs-lookup"><span data-stu-id="4edc2-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="4edc2-114">Posuňte sa nadol na službu WebClient a skontrolujte, či sa v stĺpci **stav** zobrazuje text spustiť.</span><span class="sxs-lookup"><span data-stu-id="4edc2-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="4edc2-115">Ak to tak nie je, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="4edc2-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4edc2-116">(Ak chcete službu najskôr povoliť, vyberte možnosť **manuálne** alebo **Automatické** v poli **Typ spustenia** .)</span><span class="sxs-lookup"><span data-stu-id="4edc2-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4edc2-117">Otvorenie knižnice v Prieskumníkovi je užitočné v prípade, ak je potrebné skopírovať alebo premiestniť viacero súborov a priečinkov raz, ale ak chcete pravidelne pracovať v knižnici, odporúčame ju synchronizovať.</span><span class="sxs-lookup"><span data-stu-id="4edc2-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="4edc2-118">Ak chcete riešiť problémy pri otváraní v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="4edc2-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4edc2-119">Informácie o nastavení synchronizácie nájdete v téme [Synchronizácia súborov SharePointu s novým synchronizačným klientom pre OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4edc2-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="4edc2-120">Ďalšie informácie nájdete v článku [používanie príkazu Otvoriť v programe Prieskumník na riešenie problémov v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="4edc2-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

