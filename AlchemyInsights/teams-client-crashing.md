---
title: Klient Teams zlyháva?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826286"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e254a-102">Klient Teams zlyháva?</span><span class="sxs-lookup"><span data-stu-id="e254a-102">Teams client crashing?</span></span>

<span data-ttu-id="e254a-103">Ak váš klient Teams zlyháva, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="e254a-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e254a-104">Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e254a-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e254a-105">Skontrolujte, či sú všetky URL adresy a rozsahy adries v Microsoft [365](https://docs.microsoft.com/microsoftteams/connectivity-issues) prístupné.</span><span class="sxs-lookup"><span data-stu-id="e254a-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e254a-106">Prihláste sa pomocou svojho konta správcu nájomníka a skontrolujte tabuľu [stavu](https://docs.microsoft.com/office365/enterprise/view-service-health) služby a overte, či k dispozícii nie sú žiadne výpadky ani zníženie úrovne služieb.</span><span class="sxs-lookup"><span data-stu-id="e254a-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="e254a-107">Odinštalovanie a opätovné nainštalovanie aplikácie Teams (prepojenie)</span><span class="sxs-lookup"><span data-stu-id="e254a-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="e254a-108">Prejdite do priečinka %appdata%\Microsoft\teams\ v počítači a odstráňte všetky súbory v tomto adresári.</span><span class="sxs-lookup"><span data-stu-id="e254a-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="e254a-109">[Stiahnite a nainštalujte aplikáciu Teams.](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)Ak je to možné, nainštalujte si Teams ako správca (kliknite pravým tlačidlom myši na inštalátor aplikácie Teams a vyberte možnosť "Spustiť ako správca", ak je k dispozícii).</span><span class="sxs-lookup"><span data-stu-id="e254a-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="e254a-110">Ak váš klient Teams stále zlyháva, môžete problém reprodukovať?</span><span class="sxs-lookup"><span data-stu-id="e254a-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="e254a-111">Ak áno:</span><span class="sxs-lookup"><span data-stu-id="e254a-111">If so:</span></span>

1. <span data-ttu-id="e254a-112">Pomocou diktafónu krokov zaznamenajte svoje kroky.</span><span class="sxs-lookup"><span data-stu-id="e254a-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e254a-113">Zavrite všetky nepotrebné alebo dôverné aplikácie.</span><span class="sxs-lookup"><span data-stu-id="e254a-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e254a-114">Spustite záznam krokov a reprodukovať problém, keď ste prihlásení pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="e254a-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="e254a-115">[Zhromaždite záznamy o tímoch, ktoré zaznamenávajú zaznamenané kroky opätovného zabezpečenia.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="e254a-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="e254a-116">**Poznámka:** Nezabudnite zaznamenať prihlasovaciu adresu o vplyve používateľa.</span><span class="sxs-lookup"><span data-stu-id="e254a-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="e254a-117">Zhromaždenie informácií o výpise alebo chybe kontajnera (Windows).</span><span class="sxs-lookup"><span data-stu-id="e254a-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="e254a-118">Spustite prostredie Windows Powershell v počítači, v ktorom dochádza k zlyhaiu, a spustite nasledujúce príkazy:</span><span class="sxs-lookup"><span data-stu-id="e254a-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="e254a-119">Priložte súbor k prípadu podpory.</span><span class="sxs-lookup"><span data-stu-id="e254a-119">Attach the file to your support case.</span></span>
