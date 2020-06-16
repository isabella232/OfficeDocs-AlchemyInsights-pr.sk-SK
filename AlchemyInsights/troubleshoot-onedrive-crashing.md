---
title: Riešenie problémov s onedrivom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749168"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e860e-102">Riešenie problémov s onedrivom</span><span class="sxs-lookup"><span data-stu-id="e860e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e860e-103">Ak OneDrive opakovane zlyhá, vyskúšajte tieto kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="e860e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e860e-104">**Uistite sa, že kľúče databázy registry nie sú nastavené:**</span><span class="sxs-lookup"><span data-stu-id="e860e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e860e-105">Pomocou Editora databázy Registry prejdite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e860e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e860e-106">Ak DisableFileSyncNGSC je prítomný a nastavená na 1, otvorte kľúč a zmeňte hodnotu 0.</span><span class="sxs-lookup"><span data-stu-id="e860e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e860e-107">Manuálne spustenie OneDrivu prechodom na domovskú obrazovku</span><span class="sxs-lookup"><span data-stu-id="e860e-107">Manually launch OneDrive by going to Start</span></span> ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e860e-109">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e860e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e860e-110">**Obnovenie onedrivu:**</span><span class="sxs-lookup"><span data-stu-id="e860e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e860e-111">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="e860e-111">Notes:</span></span>

- <span data-ttu-id="e860e-112">Obnovením výrobných nastavení OneDrivu sa odpojí všetky existujúce pripojenia synchronizácie (vrátane osobného OneDrivu, ak je nastavený).</span><span class="sxs-lookup"><span data-stu-id="e860e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e860e-113">Nestratíte súbory ani údaje obnovením nastavenia OneDrivu v počítači.</span><span class="sxs-lookup"><span data-stu-id="e860e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e860e-114">**Obnovenie nastavenia OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="e860e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e860e-115">Stlačením klávesu s logom Windows a R otvorte dialógové okno Spustiť.</span><span class="sxs-lookup"><span data-stu-id="e860e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e860e-116">Zadajte reťazec %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stlačte tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="e860e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e860e-117">Krátko sa môže zobraziť okno príkazu.</span><span class="sxs-lookup"><span data-stu-id="e860e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e860e-118">Manuálne spustenie OneDrivu prechodom na domovskú obrazovku</span><span class="sxs-lookup"><span data-stu-id="e860e-118">Manually launch OneDrive by going to Start</span></span> ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e860e-120">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e860e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e860e-121">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="e860e-121">Notes:</span></span>

- <span data-ttu-id="e860e-122">Ak ste sa rozhodli synchronizovať iba niektoré priečinky pred obnovením, budete musieť urobiť znova po dokončení synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="e860e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e860e-123">Ďalšie informácie nájdete v téme [Výber priečinkov onedrivu, ktoré sa majú synchronizovať s počítačom.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  </span><span class="sxs-lookup"><span data-stu-id="e860e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e860e-124">Budete ho musieť dokončiť pre svoj osobný OneDrive a OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e860e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>