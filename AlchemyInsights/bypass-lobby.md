---
title: Obísť lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376825"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="73a1b-102">Ovládanie nastavení vstupnej haly a úrovne účasti</span><span class="sxs-lookup"><span data-stu-id="73a1b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="73a1b-103">Tieto nastavenia kontrolujú, ktoré účastníci stretnutia čakajú vo vstupnej hale pred tým, ako sú prijatí na schôdzu, a úroveň účasti, ktorú sú povolené na schôdzi.</span><span class="sxs-lookup"><span data-stu-id="73a1b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="73a1b-104">PowerShell môžete použiť na aktualizáciu nastavenia politiky schôdzí, ktoré ešte neboli implementované (označené ako "pripravujeme") v tíme admin Center.</span><span class="sxs-lookup"><span data-stu-id="73a1b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="73a1b-105">Pozri nižšie pre príklad rutiny cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.</span><span class="sxs-lookup"><span data-stu-id="73a1b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="73a1b-106">[Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.</span><span class="sxs-lookup"><span data-stu-id="73a1b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="73a1b-107">[Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.</span><span class="sxs-lookup"><span data-stu-id="73a1b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="73a1b-108">[Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .</span><span class="sxs-lookup"><span data-stu-id="73a1b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="73a1b-109">[Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastaví v **automatickom priznávanie osôb** a **povolenie telefonického pripojenia používateľom obísť vstupnú halu** , keď naplánujú novú schôdzu.</span><span class="sxs-lookup"><span data-stu-id="73a1b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="73a1b-110">**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="73a1b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="73a1b-111">**Príklad PowerShell**</span><span class="sxs-lookup"><span data-stu-id="73a1b-111">**PowerShell example**</span></span>

<span data-ttu-id="73a1b-112">Ak chcete umožniť všetkým, vrátane externých alebo anonymných používateľov, obísť lobby, môžete tiež použiť PowerShell na splnenie tejto úlohy.</span><span class="sxs-lookup"><span data-stu-id="73a1b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="73a1b-113">Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="73a1b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="73a1b-114">(Nezabudnite skontrolovať dokumentáciu vyššie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.)</span><span class="sxs-lookup"><span data-stu-id="73a1b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="73a1b-115">Súbor CsTeamsMeetingPolicy-identita globálne-AutoAdmittedUsers "každý"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="73a1b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="73a1b-116">Ďalšie informácie nájdete v téme [súbor CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="73a1b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
