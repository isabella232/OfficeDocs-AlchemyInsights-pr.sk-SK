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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626363"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="36f55-102">Ovládanie nastavení vstupnej haly a úrovne účasti</span><span class="sxs-lookup"><span data-stu-id="36f55-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="36f55-103">Ak chcete povoliť všetkým, vrátane dial-in, externých a anonymných používateľov obísť lobby v Microsoft Teams, môžete použiť PowerShell na to.</span><span class="sxs-lookup"><span data-stu-id="36f55-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="36f55-104">Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu:</span><span class="sxs-lookup"><span data-stu-id="36f55-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="36f55-105">Tento cmdlet v súčasnosti vyžaduje použitie Skype Business PowerShell modulu.</span><span class="sxs-lookup"><span data-stu-id="36f55-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="36f55-106">Ak chcete získať nastavenie na používanie tejto rutiny cmdlet, pozrite si [správu politík pomocou prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="36f55-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="36f55-107">Môžete nastaviť novú politiku, ktorú potom budete musieť použiť pre používateľov.</span><span class="sxs-lookup"><span data-stu-id="36f55-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="36f55-108">Ak upravíte globálnu politiku, ktorá sa automaticky použije pre používateľov.</span><span class="sxs-lookup"><span data-stu-id="36f55-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="36f55-109">Pre každú zmenu politiky musíte počkať aspoň 4 hodiny a až 24 hodín, kým sa politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="36f55-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="36f55-110">Nezabudnite si prezrieť dokumentáciu nižšie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.</span><span class="sxs-lookup"><span data-stu-id="36f55-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="36f55-111">Pochopenie tímov pre kontrolu politiky lobby</span><span class="sxs-lookup"><span data-stu-id="36f55-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="36f55-112">[Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.</span><span class="sxs-lookup"><span data-stu-id="36f55-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="36f55-113">[Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.</span><span class="sxs-lookup"><span data-stu-id="36f55-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="36f55-114">[Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .</span><span class="sxs-lookup"><span data-stu-id="36f55-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="36f55-115">[Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastala v **automatickom priznávanie ľudí** a **umožniť používateľom telefonického pripojenia, aby pri plánovaní novej schôdze obchádzali vstupnú halu** .</span><span class="sxs-lookup"><span data-stu-id="36f55-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="36f55-116">**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="36f55-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
