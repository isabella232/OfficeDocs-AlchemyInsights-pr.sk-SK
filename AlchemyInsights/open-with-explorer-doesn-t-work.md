---
title: Open s Explorer nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28310602"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="353d6-102">Open s Explorer nefunguje</span><span class="sxs-lookup"><span data-stu-id="353d6-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="353d6-p101">Ak **Otvoriť v programe Prieskumník** alebo **v Prieskumníkovi** nepomôže uistite sa, že služba WebClient nastavená na **Spustenie** pomocou nasledujúcich krokov. Napríklad to môže trvať dlhú dobu na otvorenie knižnice SharePoint alebo OneDrive, keď služba nie je spustená.</span><span class="sxs-lookup"><span data-stu-id="353d6-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="353d6-105">Windows vyhľadávacieho poľa zadajte text spustiť, vyberte počítačovú aplikáciu spustiť, zadajte príkaz services.msc a potom stlačte **kláves Enter**.</span><span class="sxs-lookup"><span data-stu-id="353d6-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="353d6-p102">Prejdite na službu WebClient a skontrolujte **stav** stĺpec. Ak stav služby WebClient nie je **spustený**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**. Zapnutie služby, v prípade potreby výberom **vybertemanuálne** alebo **Automatické** v poli **Typ spustenia** .</span><span class="sxs-lookup"><span data-stu-id="353d6-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="353d6-p103">Riešenie problémov otvoriť v programe Prieskumník, pozrite si [Otvoriť v programe Prieskumník](https://go.microsoft.com/fwlink/?linkid=871665). Preskúmajte synchronizácie ako lepšiu alternatívu: [synchronizovať SharePoint súbory pomocou nového klienta synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="353d6-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

