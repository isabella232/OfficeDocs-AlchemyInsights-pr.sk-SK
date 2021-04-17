---
title: Riešenie problémov so zlyhaním OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826214"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="011e9-102">Riešenie problémov so zlyhaním OneDrivu</span><span class="sxs-lookup"><span data-stu-id="011e9-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="011e9-103">Ak OneDrive opakovane zlyhá, vyskúšajte tieto kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="011e9-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="011e9-104">**Presvedčte sa, že kľúče databázy Registry nie sú nastavené:**</span><span class="sxs-lookup"><span data-stu-id="011e9-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="011e9-105">Pomocou Editora databázy Registry prejdite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="011e9-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="011e9-106">Ak je k dispozícii DisableFileSyncNGSC a je nastavený na možnosť 1, otvorte kľúč a zmeňte hodnotu na 0.</span><span class="sxs-lookup"><span data-stu-id="011e9-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="011e9-107">Manuálne spustenie OneDrivu pomocou ponuky Štart</span><span class="sxs-lookup"><span data-stu-id="011e9-107">Manually launch OneDrive by going to Start</span></span> ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="011e9-109">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="011e9-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="011e9-110">**Vynulovanie nastavenia pre OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="011e9-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="011e9-111">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="011e9-111">Notes:</span></span>

- <span data-ttu-id="011e9-112">Vynulovaním nastavenia pre OneDrive sa odpoja všetky existujúce synchronizačné pripojenia (vrátane vášho osobného konta vo OneDrive, ak ho máte nastavené).</span><span class="sxs-lookup"><span data-stu-id="011e9-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="011e9-113">Vynulovaním nastavení služby OneDrive v počítači nestratíte žiadne súbory ani údaje.</span><span class="sxs-lookup"><span data-stu-id="011e9-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="011e9-114">**Vynulovanie nastavenia pre OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="011e9-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="011e9-115">Otvorte dialógové okno Spustiť stlačením klávesu s logom Windows a klávesu R.</span><span class="sxs-lookup"><span data-stu-id="011e9-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="011e9-116">Zadajte príkaz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stlačte tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="011e9-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="011e9-117">Na chvíľu sa môže zobraziť okno Príkazový riadok.</span><span class="sxs-lookup"><span data-stu-id="011e9-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="011e9-118">Manuálne spustenie OneDrivu pomocou ponuky Štart</span><span class="sxs-lookup"><span data-stu-id="011e9-118">Manually launch OneDrive by going to Start</span></span> ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="011e9-120">, do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="011e9-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="011e9-121">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="011e9-121">Notes:</span></span>

- <span data-ttu-id="011e9-122">Ak ste pred vynulním nastavení vybrali synchronizáciu iba niektorých priečinkov, budete to po synchronizácii musieť urobiť ešte raz.</span><span class="sxs-lookup"><span data-stu-id="011e9-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="011e9-123">Ďalšie [informácie nájdete v článku Výber priečinkov OneDrivu na synchronizáciu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)s   počítačom.</span><span class="sxs-lookup"><span data-stu-id="011e9-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="011e9-124">Tento problém budete musieť dokončiť pre svoj osobný OneDrive a OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="011e9-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>