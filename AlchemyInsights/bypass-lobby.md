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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889097"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="51c19-102">Ovládanie nastavení vstupnej haly a úrovne účasti v tímoch</span><span class="sxs-lookup"><span data-stu-id="51c19-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="51c19-103">Ak chcete povoliť všetkým, vrátane dial-in, externých a anonymných používateľov, **obísť lobby**, použite PowerShell na splnenie tejto úlohy.</span><span class="sxs-lookup"><span data-stu-id="51c19-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="51c19-104">Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="51c19-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="51c19-105">Tento cmdlet v súčasnosti vyžaduje použitie Skype Business PowerShell modulu.</span><span class="sxs-lookup"><span data-stu-id="51c19-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="51c19-106">Ak chcete nastaviť použitie tejto rutiny cmdlet, pozrite sa na [správu politík pomocou prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="51c19-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="51c19-107">Po nastavení politiky ju musíte aplikovať na používateľov. alebo ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov.</span><span class="sxs-lookup"><span data-stu-id="51c19-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="51c19-108">Pri každej zmene politiky musíte počkať aspoň **4 hodiny až 24 hodín** , kým sa politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="51c19-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="51c19-109">Nezabudnite si prezrieť dokumentáciu nižšie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.</span><span class="sxs-lookup"><span data-stu-id="51c19-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="51c19-110">Pochopenie tímov pre kontrolu politiky lobby</span><span class="sxs-lookup"><span data-stu-id="51c19-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="51c19-111">Tieto nastavenia kontrolujú, ktoré účastníci stretnutia čakajú vo vstupnej hale pred tým, ako sú prijatí na schôdzu, a úroveň účasti, ktorú sú povolené na schôdzi.</span><span class="sxs-lookup"><span data-stu-id="51c19-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="51c19-112">PowerShell môžete použiť na aktualizáciu nastavenia politiky schôdzí, ktoré ešte neboli implementované (označené ako "pripravujeme") v tíme admin Center.</span><span class="sxs-lookup"><span data-stu-id="51c19-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="51c19-113">Pozri nižšie pre príklad rutiny cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.</span><span class="sxs-lookup"><span data-stu-id="51c19-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="51c19-114">[Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.</span><span class="sxs-lookup"><span data-stu-id="51c19-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="51c19-115">[Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.</span><span class="sxs-lookup"><span data-stu-id="51c19-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="51c19-116">[Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .</span><span class="sxs-lookup"><span data-stu-id="51c19-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="51c19-117">[Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastala v **automatickom priznávanie ľudí** a **umožniť používateľom telefonického pripojenia, aby pri plánovaní novej schôdze obchádzali vstupnú halu** .</span><span class="sxs-lookup"><span data-stu-id="51c19-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="51c19-118">**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="51c19-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
