---
title: Riešenie problémov s programom otvoriť v programe Prieskumník
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742748"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="54c3b-102">Riešenie problémov s programom Open Explorer</span><span class="sxs-lookup"><span data-stu-id="54c3b-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="54c3b-103">Oprava bežných problémov s otvorením knižnice dokumentov v SharePointe alebo OneDrive pomocou príkazu **Otvoriť v programe Prieskumník** :</span><span class="sxs-lookup"><span data-stu-id="54c3b-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="54c3b-104">Použite Internet Explorer 10 alebo Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="54c3b-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="54c3b-105">**Otvoriť v programe Prieskumník** nie je kompatibilný s prehliadačom Microsoft Edge, Google Chrome, Firefox a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="54c3b-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="54c3b-106">**Otvoriť v programe Prieskumník** je vypnutá vo všetkých prehliadačoch okrem Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="54c3b-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="54c3b-107">**Otvoriť v programe Prieskumník** nie je k dispozícii v modernom zážitku pre knižnice SharePoint.</span><span class="sxs-lookup"><span data-stu-id="54c3b-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="54c3b-108">Namiesto toho použite **Zobraziť v Prieskumníkovi** .</span><span class="sxs-lookup"><span data-stu-id="54c3b-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="54c3b-109">**V Prieskumníkovi**vyberte zobrazenie **Možnosti** \> zobrazenia.</span><span class="sxs-lookup"><span data-stu-id="54c3b-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="54c3b-110">Zobrazenie v Prieskumníkovi nie je kompatibilné s prehliadačom Microsoft Edge, Google Chrome, Firefox a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="54c3b-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="54c3b-111">**Zobrazenie v Prieskumníkovi** dostupné iba v programe Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="54c3b-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="54c3b-112">Uistite sa, že je spustená služba WebClient.</span><span class="sxs-lookup"><span data-stu-id="54c3b-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="54c3b-113">Do poľa Hľadať v systéme Windows zadajte príkaz Spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte príkaz Services. msc a stlačte kláves ENTER.</span><span class="sxs-lookup"><span data-stu-id="54c3b-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="54c3b-114">Posuňte sa nadol na službu WebClient a uistite sa, že v stĺpci **stav** sa zobrazuje "beh".</span><span class="sxs-lookup"><span data-stu-id="54c3b-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="54c3b-115">Ak sa tak nestane, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="54c3b-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="54c3b-116">(Musíte najprv povoliť službu výberom buď **manuálne** alebo **Automatické** v **Typ spustenia** rámček.)</span><span class="sxs-lookup"><span data-stu-id="54c3b-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="54c3b-117">Otvorenie knižnice v Prieskumníkovi je užitočné, ak potrebujete skopírovať alebo premiestniť viacero súborov a priečinkov raz, ale ak chcete pravidelne pracovať v knižnici, odporúčame synchronizáciu.</span><span class="sxs-lookup"><span data-stu-id="54c3b-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="54c3b-118">Ak chcete riešiť problémy s otvorením v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="54c3b-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="54c3b-119">Informácie o nastavení synchronizácie nájdete [v téme Synchronizácia súborov SharePoint s novým klientom synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="54c3b-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="54c3b-120">Prečítajte si článok [ako používať príkaz "otvoriť v programe Prieskumník" na riešenie problémov SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="54c3b-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

