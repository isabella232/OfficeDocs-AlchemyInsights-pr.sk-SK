---
title: Teams klient zlyháva
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187736"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="8ed1b-102">Teams klient zlyháva</span><span class="sxs-lookup"><span data-stu-id="8ed1b-102">Teams client crashing</span></span>

<span data-ttu-id="8ed1b-103">Ak váš klient Teams zlyháva, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="8ed1b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="8ed1b-104">Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="8ed1b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="8ed1b-105">Skontrolujte, či sú [všetky Microsoft 365 URL adresy a rozsahy adries](/microsoftteams/connectivity-issues) prístupné.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="8ed1b-106">Prihláste sa pomocou svojho konta správcu nájomníka a skontrolujte tabuľu [stavu](/office365/enterprise/view-service-health) služby a overte, či k dispozícii nie sú žiadne výpadky ani zníženie úrovne služieb.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="8ed1b-107">Odinštalovanie a opätovné nainštalovanie Teams aplikácie</span><span class="sxs-lookup"><span data-stu-id="8ed1b-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="8ed1b-108">Prejdite do priečinka %appdata%\Microsoft\Teams\ v počítači a odstráňte všetky súbory z tohto adresára.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="8ed1b-109">[Stiahnite](https://www.microsoft.com/microsoft-teams/download-app)a nainštalujte Teams App a ak je to možné, nainštalujte Teams ako správca (kliknite pravým tlačidlom myši na inštalátor balíka Teams a vyberte položku Spustiť ako **správca,** ak je k dispozícii).</span><span class="sxs-lookup"><span data-stu-id="8ed1b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="8ed1b-110">Ak Teams klienta stále zlyháva, pokúste sa problém reprodukovať.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="8ed1b-111">Ak môžete:</span><span class="sxs-lookup"><span data-stu-id="8ed1b-111">If you can:</span></span>

1. <span data-ttu-id="8ed1b-112">Pomocou diktafónu krokov zaznamenajte svoje kroky.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="8ed1b-113">Zavrite všetky nepotrebné alebo dôverné aplikácie.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="8ed1b-114">Spustite záznam krokov a reprodukovať problém, keď ste prihlásení pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="8ed1b-115">[Zhromaždite záznamy o tímoch, ktoré zaznamenávajú zaznamenané kroky opätovného zabezpečenia.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="8ed1b-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="8ed1b-116">**Poznámka:** Nezabudnite zaznamenať prihlasovaciu adresu o vplyve používateľa.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="8ed1b-117">Zhromaždenie informácií o výpise alebo chybe kontajnera (Windows).</span><span class="sxs-lookup"><span data-stu-id="8ed1b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="8ed1b-118">Spustite Windows PowerShell v počítači, v ktorom sa vyskytuje zlyhanie, a spustite nasledujúce príkazy (po každom príkaze stlačte kláves Enter):</span><span class="sxs-lookup"><span data-stu-id="8ed1b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="8ed1b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="8ed1b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="8ed1b-120">Po vygenerovaní textového súboru, ktorý sa zobrazí na obrazovke, uložte súbor a priložte ho k žiadosti o službu.</span><span class="sxs-lookup"><span data-stu-id="8ed1b-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
