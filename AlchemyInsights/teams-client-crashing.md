---
title: Klient Teams zlyháva?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030673"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="90633-102">Klient Teams zlyháva?</span><span class="sxs-lookup"><span data-stu-id="90633-102">Teams client crashing?</span></span>

<span data-ttu-id="90633-103">Ak váš klient Teams zlyháva, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="90633-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="90633-104">Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="90633-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="90633-105">Uistite sa, že všetky [URL adresy a rozsahy adries služby Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sú dostupné.</span><span class="sxs-lookup"><span data-stu-id="90633-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="90633-106">Prihláste sa so svojím kontom správcu a na [tabuli stavu služby](https://docs.microsoft.com/office365/enterprise/view-service-health) overte, či nedochádza k výpadku alebo zhoršeniu služby.</span><span class="sxs-lookup"><span data-stu-id="90633-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="90633-107">Ako posledný krok sa môžete pokúsiť vymazať vyrovnávaciu pamäť klienta Teams:</span><span class="sxs-lookup"><span data-stu-id="90633-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="90633-108">Úplne ukončite počítačového klienta Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="90633-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="90633-109">Môžete kliknúť pravým tlačidlom myši na ikonu **Teams** na paneli úloh a kliknúť na položku **Ukončiť** alebo spustiť správcu úloh a ukončiť proces.</span><span class="sxs-lookup"><span data-stu-id="90633-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="90633-110">Prejdite do Prieskumníka a zadajte %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="90633-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="90633-111">Keď sa budete nachádzať v uvedenom adresári, zobrazia sa niektoré z týchto priečinkov:</span><span class="sxs-lookup"><span data-stu-id="90633-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="90633-112">V priečinku **Application Cache** prejdite do priečinka Cache a odstráňte všetky súbory v priečinku Cache: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="90633-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="90633-113">V priečinku **Blob_storage** odstráňte všetky súbory: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="90633-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="90633-114">V priečinku **Cache** odstráňte všetky súbory: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="90633-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="90633-115">V priečinku **databases** odstráňte všetky súbory: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="90633-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="90633-116">V priečinku **GPUCache** odstráňte všetky súbory: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="90633-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="90633-117">V priečinku **IndexedDB** odstráňte súbor .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="90633-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="90633-118">V priečinku **Local Storage** odstráňte všetky súbory: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="90633-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="90633-119">A napokon v priečinku **tmp** odstráňte všetky súbory: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="90633-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="90633-120">Znova spustite klienta Teams.</span><span class="sxs-lookup"><span data-stu-id="90633-120">Restart your Teams client.</span></span>
