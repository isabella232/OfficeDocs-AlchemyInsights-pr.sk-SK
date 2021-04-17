---
title: Obídenie čakáreň
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820049"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="9a389-102">Ovládanie nastavení čakáreň a úrovne účasti v Teams</span><span class="sxs-lookup"><span data-stu-id="9a389-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="9a389-103">Ak chcete všetkým vrátane telefonických, externých a anonymných používateľov povoliť obídenie čakáreň **,** použite prostredie PowerShell na vykonanie tejto úlohy.</span><span class="sxs-lookup"><span data-stu-id="9a389-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="9a389-104">Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="9a389-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="9a389-105">Táto rutina typu cmdlet momentálne vyžaduje používanie modulu Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9a389-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="9a389-106">Ak chcete nastaviť používanie tejto rutiny typu cmdlet, pozrite si časť [Spravovanie politík prostredníctvom prostredia PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="9a389-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="9a389-107">Po nastavení politiky ju budete musieť použiť pre používateľov. alebo, ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov.</span><span class="sxs-lookup"><span data-stu-id="9a389-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="9a389-108">Pri každej zmene politiky je potrebné počkať aspoň 4 hodiny až **do 24** hodín, kým sa politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="9a389-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="9a389-109">Pred vykonaním týchto zmien nezabudnite skontrolovať dokumentáciu nižšie, aby ste presne pochopili, čo to umožňuje.</span><span class="sxs-lookup"><span data-stu-id="9a389-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="9a389-110">Vysvetlenie ovládacích prvkov politiky čakární schôdze cez Teams</span><span class="sxs-lookup"><span data-stu-id="9a389-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="9a389-111">Tieto nastavenia ovládajú, ktorí účastníci schôdze pred ich vstupom na schôdzu budú čakať v čakárni, a tiež povolenú úroveň účasti na schôdzi.</span><span class="sxs-lookup"><span data-stu-id="9a389-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="9a389-112">Pomocou prostredia PowerShell môžete aktualizovať nastavenia politiky schôdze, ktoré ešte neboli implementované (označené ako čoskoro k dispozícii) v Centre spravovania pre Teams.</span><span class="sxs-lookup"><span data-stu-id="9a389-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="9a389-113">Nižšie je uvedený príklad rutiny typu cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť čakáreň.</span><span class="sxs-lookup"><span data-stu-id="9a389-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="9a389-114">[Automatické prijatie osôb je](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) politika organizátora, ktorá určuje, či sa ľudia pripájajú k schôdzi priamo alebo počkať v čakárni, kým ich nepripojí overený používateľ.</span><span class="sxs-lookup"><span data-stu-id="9a389-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9a389-115">[Umožniť](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) anonymným ľuďom začať schôdzu je politika organizátora, ktorá určuje, či sa anonymní ľudia vrátane B2B a federované používatelia môžu pripojiť k schôdzi používateľa bez toho, aby z organizácie používala účasť overený používateľ.</span><span class="sxs-lookup"><span data-stu-id="9a389-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9a389-116">[Povoliť používateľom](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) telefonickej konferencie obísť čakáreň **(čoskoro** k dispozícii) je politika organizátora, ktorá určuje, či sa používatelia telefonicky pripoja k schôdzi priamo alebo čakajú v čakárni bez ohľadu na nastavenie Automaticky **prijať** ľudí.</span><span class="sxs-lookup"><span data-stu-id="9a389-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9a389-117">[Možnosť Povoliť organizátorom](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) prepísať nastavenia čakáreň **(čoskoro** k dispozícii) je politika organizátora, ktorá  určuje,  či organizátor schôdze môže prepísať nastavenia čakáreň, ktoré správca nastavil v časti Automaticky prijať osoby a Povoliť používateľom telefonickej konferencie obísť čakáreň pri naplánovaní novej schôdze.</span><span class="sxs-lookup"><span data-stu-id="9a389-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9a389-118">**Poznámka:** Úplný [prehľad politík schôdzí v aplikácii](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Microsoft Teams nájdete v článku Spravovanie politík schôdzí v aplikácii Teams.</span><span class="sxs-lookup"><span data-stu-id="9a389-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
