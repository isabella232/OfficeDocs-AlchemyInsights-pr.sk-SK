---
title: Riešenie problémov pomocou Open Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489247"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="062cc-102">Riešenie problémov s Open s Explorer</span><span class="sxs-lookup"><span data-stu-id="062cc-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="062cc-103">Vyriešiť bežné problémy s otváraním knižnica dokumentov SharePoint alebo OneDrive pomocou príkazu **Otvoriť v programe Prieskumník** :</span><span class="sxs-lookup"><span data-stu-id="062cc-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="062cc-p101">Pomocou programu Internet Explorer 10 alebo Internet Explorer 11. **Otvoriť v programe Prieskumník** nie je kompatibilný s Microsoft Edge, prehliadač Google Chrome, Firefox a ďalšie. **Open s Explorer** vypnutá vo všetkých prehliadačoch okrem programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="062cc-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="062cc-p102">**Otvoriť v programe Prieskumník** nie je k dispozícii v modernej skúsenosti pre knižnice. Použite **zobrazenie v Prieskumníkovi** . Vyberte **Zobraziť možnosti** \> **zobrazenie v Prieskumníkovi**. Zobrazenie v Prieskumníkovi súborov nie je kompatibilný s Microsoft Edge, prehliadač Google Chrome, Firefox a ďalšie. **Zobrazenie v Prieskumníkovi súborov** k dispozícii len v programe Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="062cc-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="062cc-p103">Uistite sa, že je spustená služba WebClient. Do poľa Hľadať systém Windows zadajte spustiť, vyberte počítačovú aplikáciu spustiť, zadajte services.msc a stlačte kláves Enter. Prejdite na službu WebClient a skontrolujte **stav** stĺpec zobrazí "Beží." Ak nie, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**. (Musíte najprv zapnúť službu výberom buď **manuálne** alebo **automaticky** v **Typ spustenia** políčka.)</span><span class="sxs-lookup"><span data-stu-id="062cc-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="062cc-p104">Otvorenie knižnice v programe Prieskumník sa hodí, ak potrebujete na kopírovanie alebo presúvanie viacerých súborov a priečinkov, akonáhle, ale ak chcete pravidelne pracovať v knižnici, odporúčame vám jeho synchronizáciu. Riešenie problémov otvoriť v programe Prieskumník, pozrite si [Otvoriť v programe Prieskumník](https://go.microsoft.com/fwlink/?linkid=871665). Informácie o nastavení synchronizácie, pozrite si [synchronizovať SharePoint súbory pomocou nového klienta synchronizácie OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="062cc-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="062cc-120">Prečítajte si článok [ako používať príkaz "Open s Explorer" riešenie problémov v službe SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="062cc-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

