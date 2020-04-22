---
title: Otvoriť v programe Prieskumník nefunguje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713049"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="9f3dd-102">Otvoriť v programe Prieskumník nefunguje</span><span class="sxs-lookup"><span data-stu-id="9f3dd-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="9f3dd-103">Ak **Otvoriť v programe Prieskumník** alebo **Zobraziť v Prieskumníkovi** nefunguje uistite sa, že služba WebClient je nastavená na **spúšťanie** podľa nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="9f3dd-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="9f3dd-104">Napríklad, to môže trvať dlho otvoriť SharePoint alebo OneDrive knižnice, keď služba nie je spustená.</span><span class="sxs-lookup"><span data-stu-id="9f3dd-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="9f3dd-105">Do poľa Hľadať v systéme Windows zadajte príkaz Spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte príkaz Services. msc a potom vyberte položku **Enter (zadať**).</span><span class="sxs-lookup"><span data-stu-id="9f3dd-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="9f3dd-106">Posuňte sa nadol na službu WebClient a skontrolujte **stavový** stĺpec.</span><span class="sxs-lookup"><span data-stu-id="9f3dd-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="9f3dd-107">Ak stav služby WebClient nie je **spustená**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**, a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="9f3dd-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9f3dd-108">Ak je to potrebné, povoľte službu výberom položky **manuálne** alebo **automaticky** v poli **Typ spustenia** .</span><span class="sxs-lookup"><span data-stu-id="9f3dd-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9f3dd-109">Ak chcete riešiť problémy s otvorením v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9f3dd-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9f3dd-110">Preskúmajte synchronizáciu ako lepšiu alternatívu: [Synchronizujte súbory SharePoint s novým klientom synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9f3dd-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

