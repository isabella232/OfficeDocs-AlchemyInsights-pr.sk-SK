---
title: Open s Explorer nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538501"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="5fbf3-102">Open s Explorer nefunguje</span><span class="sxs-lookup"><span data-stu-id="5fbf3-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="5fbf3-103">Ak **Otvoriť v programe Prieskumník** alebo **v Prieskumníkovi** nepomôže uistite sa, že služba WebClient nastavená na **Spustenie** pomocou nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="5fbf3-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="5fbf3-104">Napríklad to môže trvať dlhú dobu na otvorenie knižnice SharePoint alebo OneDrive, keď služba nie je spustená.</span><span class="sxs-lookup"><span data-stu-id="5fbf3-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="5fbf3-105">Windows vyhľadávacieho poľa zadajte text spustiť, vyberte počítačovú aplikáciu spustiť, zadajte príkaz services.msc a potom stlačte **kláves Enter**.</span><span class="sxs-lookup"><span data-stu-id="5fbf3-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="5fbf3-106">Prejdite na službu WebClient a skontrolujte **stav** stĺpec.</span><span class="sxs-lookup"><span data-stu-id="5fbf3-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="5fbf3-107">Ak stav služby WebClient nie je **spustený**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="5fbf3-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5fbf3-108">Zapnutie služby, v prípade potreby výberom **vybertemanuálne** alebo **Automatické** v poli **Typ spustenia** .</span><span class="sxs-lookup"><span data-stu-id="5fbf3-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5fbf3-109">Riešenie problémov otvoriť v programe Prieskumník, pozrite si [Otvoriť v programe Prieskumník](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5fbf3-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5fbf3-110">Preskúmajte synchronizácie ako lepšiu alternatívu: [synchronizovať SharePoint súbory pomocou nového klienta synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5fbf3-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

