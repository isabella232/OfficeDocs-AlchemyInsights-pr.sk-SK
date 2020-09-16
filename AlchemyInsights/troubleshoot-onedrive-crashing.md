---
title: Riešenie problémov s zlyhávaním OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665013"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="31cc6-102">Riešenie problémov s zlyhávaním OneDrivu</span><span class="sxs-lookup"><span data-stu-id="31cc6-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="31cc6-103">Ak OneDrive opakovane zlyháva, vyskúšajte tieto kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="31cc6-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="31cc6-104">**Uistite sa, že kľúče databázy Registry nie sú nastavené:**</span><span class="sxs-lookup"><span data-stu-id="31cc6-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="31cc6-105">Pomocou editora databázy Registry prejdite na HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="31cc6-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="31cc6-106">Ak je DisableFileSyncNGSC prítomný a nastavený na hodnotu 1, otvorte kľúč a zmeňte hodnotu na 0.</span><span class="sxs-lookup"><span data-stu-id="31cc6-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="31cc6-107">Manuálne spustenie OneDrivu prechodom na domovskú obrazovku</span><span class="sxs-lookup"><span data-stu-id="31cc6-107">Manually launch OneDrive by going to Start</span></span> ![Stlačenie klávesu s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="31cc6-109">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="31cc6-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="31cc6-110">**Obnoviť OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="31cc6-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="31cc6-111">Poznámok</span><span class="sxs-lookup"><span data-stu-id="31cc6-111">Notes:</span></span>

- <span data-ttu-id="31cc6-112">Obnovením nastavenia služby OneDrive sa odpojí všetky existujúce synchronizačné pripojenia (vrátane vášho osobného OneDrivu, ak je nastavené).</span><span class="sxs-lookup"><span data-stu-id="31cc6-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="31cc6-113">Nestratíte žiadne súbory ani údaje vykonaním nastavenia služby OneDrive v počítači.</span><span class="sxs-lookup"><span data-stu-id="31cc6-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="31cc6-114">**Obnovenie služby OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="31cc6-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="31cc6-115">Stlačením klávesu s logom Windows a klávesu R otvorte dialógové okno spustiť.</span><span class="sxs-lookup"><span data-stu-id="31cc6-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="31cc6-116">Zadajte výraz% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset a stlačte tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="31cc6-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="31cc6-117">Okno s príkazom sa môže zobraziť stručne.</span><span class="sxs-lookup"><span data-stu-id="31cc6-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="31cc6-118">Manuálne spustenie OneDrivu prechodom na domovskú obrazovku</span><span class="sxs-lookup"><span data-stu-id="31cc6-118">Manually launch OneDrive by going to Start</span></span> ![Stlačenie klávesu s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="31cc6-120">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="31cc6-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="31cc6-121">Poznámok</span><span class="sxs-lookup"><span data-stu-id="31cc6-121">Notes:</span></span>

- <span data-ttu-id="31cc6-122">Ak ste sa pred vynulovaním rozhodli synchronizovať iba niektoré priečinky, bude potrebné vykonať túto operáciu znova po dokončení synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="31cc6-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="31cc6-123">Ďalšie informácie nájdete v [téme Výber priečinkov OneDrivu, ktoré sa majú synchronizovať s počítačom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="31cc6-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="31cc6-124">Túto možnosť budete musieť vyplniť pre svoje osobné služby OneDrive a OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="31cc6-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>