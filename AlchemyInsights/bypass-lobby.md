---
title: Obchvatová loby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684965"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="5750d-102">Ovládanie nastavení lobby a úrovne účasti v aplikácii teams</span><span class="sxs-lookup"><span data-stu-id="5750d-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="5750d-103">Ak chcete všetkým, vrátane telefonických, externých a anonymných používateľov povoliť, aby sa **vyhli vstupnej hale**, použite prostredie PowerShell na vykonanie tejto úlohy.</span><span class="sxs-lookup"><span data-stu-id="5750d-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="5750d-104">Tu je príklad úpravy globálnej politiky schôdze pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="5750d-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5750d-105">Táto rutina typu cmdlet v súčasnosti vyžaduje používanie modulu PowerShell v Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="5750d-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5750d-106">Ak chcete nastaviť používanie tejto rutiny typu cmdlet, pozrite si tému [Správa politík pomocou prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="5750d-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="5750d-107">Po nastavení politiky je potrebné ju použiť pre používateľov. Ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov.</span><span class="sxs-lookup"><span data-stu-id="5750d-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="5750d-108">Pri každej zmene politiky musíte počkať aspoň **4 hodiny až 24 hodín** , kým sa politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="5750d-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="5750d-109">Pred vykonaním týchto zmien si prečítajte dokumentáciu nižšie, aby ste presne pochopili, čo to umožňuje.</span><span class="sxs-lookup"><span data-stu-id="5750d-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5750d-110">Informácie o ovládacích prvkoch v lobby schôdze v aplikácii teams</span><span class="sxs-lookup"><span data-stu-id="5750d-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="5750d-111">Tieto nastavenia určujú, ktorí účastníci schôdze čakajú v lobby pred prijatím na schôdzu a úrovňou účasti, ktorú sú na schôdzi povolené.</span><span class="sxs-lookup"><span data-stu-id="5750d-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5750d-112">Pomocou prostredia PowerShell môžete aktualizovať nastavenia politiky schôdze, ktoré ešte neboli implementované (označené ako "čoskoro") v centre spravovania pre teams.</span><span class="sxs-lookup"><span data-stu-id="5750d-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="5750d-113">Nižšie nájdete príklad rutiny typu cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.</span><span class="sxs-lookup"><span data-stu-id="5750d-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="5750d-114">[Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú na základe politiky organizátora, ktorá kontroluje, či sa ľudia priamo pripoja k schôdzi alebo čakajú v lobby, až kým neprijmú overeného používateľa.</span><span class="sxs-lookup"><span data-stu-id="5750d-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5750d-115">[Povoliť anonymným používateľom začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je politika v rámci organizátora, ktorá určuje, či sa majú anonymné osoby vrátane B2B a externých používateľov pripájať k schôdzi používateľa bez overeného používateľa z organizácie v dochádzke.</span><span class="sxs-lookup"><span data-stu-id="5750d-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5750d-116">[Povoliť používateľom telefonických služieb obísť lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**už čoskoro**) je politika pre organizátora, ktorá kontroluje, či sa osoby, ktoré telefonicky telefonicky pripoja k schôdzi, dostávajú priamo k schôdzi alebo sa v lobby čakajú bez ohľadu na to, či sa **automaticky pripúšťa** nastavenie</span><span class="sxs-lookup"><span data-stu-id="5750d-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5750d-117">[Ak chcete, aby organizátori](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) prepísali nastavenia lobby (**už čoskoro**), je politika v rámci organizátora, ktorá kontroluje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca **automaticky priznáva ľuďom** a **Povoliť používateľom telefonických služieb obísť lobby** pri plánovaní novej schôdze.</span><span class="sxs-lookup"><span data-stu-id="5750d-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5750d-118">**Poznámka:** Prečítajte si tému [Správa politík schôdze v aplikácii teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) a získajte celkový prehľad o politikách schôdze v aplikácii Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="5750d-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
