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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354068"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="6daa1-102">Klient Teams zlyháva?</span><span class="sxs-lookup"><span data-stu-id="6daa1-102">Teams client crashing?</span></span>

<span data-ttu-id="6daa1-103">Ak váš klient Teams zlyháva, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="6daa1-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="6daa1-104">Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="6daa1-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="6daa1-105">Uistite sa, že všetky [Microsoft 365 adresy URL a rozsahy adries](https://docs.microsoft.com/microsoftteams/connectivity-issues) sú prístupné.</span><span class="sxs-lookup"><span data-stu-id="6daa1-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="6daa1-106">Prihláste sa pomocou konta správcu nájomníka a skontrolujte, či sa v [informačnom paneli služby](https://docs.microsoft.com/office365/enterprise/view-service-health) nenachádza žiadna výpadok alebo degradácia služieb.</span><span class="sxs-lookup"><span data-stu-id="6daa1-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="6daa1-107">Odinštalovanie a preinštalovanie aplikácie Teams (prepojenie)</span><span class="sxs-lookup"><span data-stu-id="6daa1-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="6daa1-108">Prejdite do priečinka%appdata%\Microsoft\teams\ v počítači a odstráňte všetky súbory v tomto adresári.</span><span class="sxs-lookup"><span data-stu-id="6daa1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="6daa1-109">[Prevezmite a nainštalujte aplikáciu teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a ak je to možné, nainštalujte tímy ako správca (kliknite pravým tlačidlom myši na Inštalátor tímov a vyberte možnosť "spustiť ako správca", ak je k dispozícii).</span><span class="sxs-lookup"><span data-stu-id="6daa1-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="6daa1-110">Ak vaše tímy klient je stále havaruje, môžete reprodukovať problém?</span><span class="sxs-lookup"><span data-stu-id="6daa1-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="6daa1-111">Ak áno:</span><span class="sxs-lookup"><span data-stu-id="6daa1-111">If so:</span></span>

1. <span data-ttu-id="6daa1-112">Použite postup rekordér zachytiť vaše kroky.</span><span class="sxs-lookup"><span data-stu-id="6daa1-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="6daa1-113">Zatvorte všetky nepotrebné alebo dôverné aplikácie.</span><span class="sxs-lookup"><span data-stu-id="6daa1-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="6daa1-114">Spustenie postupu rekordér a reprodukovať problém pri prihlásení pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="6daa1-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="6daa1-115">[Zbierať tímy denníky, ktoré zachytávajú zaznamenané repro kroky](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="6daa1-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="6daa1-116">**Poznámka**: Uistite sa, že zachytiť adresu prihlásenia ovplyvnenej používateľa.</span><span class="sxs-lookup"><span data-stu-id="6daa1-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="6daa1-117">Zhromažďovať dump a/alebo chyba vedierko info (Windows).</span><span class="sxs-lookup"><span data-stu-id="6daa1-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="6daa1-118">Spustenie prostredia Windows PowerShell na stroji, kde dochádza k zlyhaniu a spustite nasledujúce príkazy:</span><span class="sxs-lookup"><span data-stu-id="6daa1-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="6daa1-119">Priložte súbor k vášmu prípadu podpory.</span><span class="sxs-lookup"><span data-stu-id="6daa1-119">Attach the file to your support case.</span></span>
