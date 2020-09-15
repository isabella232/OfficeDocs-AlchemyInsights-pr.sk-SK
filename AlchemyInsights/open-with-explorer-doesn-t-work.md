---
title: Otvoriť v programe Prieskumník nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694471"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="7f0fd-102">Otvoriť v programe Prieskumník nefunguje</span><span class="sxs-lookup"><span data-stu-id="7f0fd-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="7f0fd-103">Ak je položka otvoriť v programe **Prieskumník** alebo **zobrazenie v Prieskumníkovi** funkčná, uistite sa, že služba WebClient je nastavená na možnosť **Spustiť** podľa nižšie uvedených krokov.</span><span class="sxs-lookup"><span data-stu-id="7f0fd-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="7f0fd-104">Pri otváraní knižnice SharePointu alebo OneDrivu môže napríklad trvať dlho, kým nie je spustená služba.</span><span class="sxs-lookup"><span data-stu-id="7f0fd-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="7f0fd-105">Do poľa Windows Search zadajte text spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte výraz Services. msc a potom vyberte položku **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7f0fd-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="7f0fd-106">Posuňte sa nadol na službu WebClient a skontrolujte stĺpec **stav** .</span><span class="sxs-lookup"><span data-stu-id="7f0fd-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="7f0fd-107">Ak stav služby WebClient nie je **spustený**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="7f0fd-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="7f0fd-108">Ak je to potrebné, zapnite službu tak, že vyberiete možnosť **manuálne** alebo **Automatické** v poli **Typ spustenia** .</span><span class="sxs-lookup"><span data-stu-id="7f0fd-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="7f0fd-109">Ak chcete riešiť problémy pri otváraní v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="7f0fd-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="7f0fd-110">Preskúmajte synchronizáciu ako lepšiu alternatívu: [Synchronizujte súbory SharePointu s novým synchronizačným klientom pre OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="7f0fd-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

