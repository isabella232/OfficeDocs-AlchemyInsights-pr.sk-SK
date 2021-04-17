---
title: Nastavenia politiky schôdze
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825458"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="fcf31-102">Spravovanie politík schôdzí v aplikácii Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fcf31-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="fcf31-103">**Poznámka: Zmeny politiky sa prejavia pre používateľov do 24 hodín.**</span><span class="sxs-lookup"><span data-stu-id="fcf31-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="fcf31-104">Je možné, že ihneď nebudete môcť vykonať zmeny v novovytvorených politikách. Počkajte 4 hodiny a skúste znova upraviť novovytvoreú politiku.</span><span class="sxs-lookup"><span data-stu-id="fcf31-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="fcf31-105">Politiky schôdzí sa používajú na ovládanie funkcií dostupných pre účastníkov schôdze na schôdze naplánované používateľmi vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="fcf31-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="fcf31-106">Niektoré funkcie politík schôdzí možno ešte nie sú implementované v Centre spravovania pre Teams (tieto sú v dokumentácii označené ako "čoskoro k dispozícii").</span><span class="sxs-lookup"><span data-stu-id="fcf31-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="fcf31-107">V tomto prípade alebo ak sa vám zobrazuje chybové hlásenie, ako napríklad "Politiku nie je možné aktualizovať hneď, ale skúste to znova neskôr" v Centre spravovania služby Microsoft Teams, odporúčame vám použiť prostredie PowerShell na vytvorenie alebo úpravu politík schôdzí cez Teams.</span><span class="sxs-lookup"><span data-stu-id="fcf31-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="fcf31-108">Ďalšie informácie o politikách schôdzí nájdete v týchto zdrojoch:</span><span class="sxs-lookup"><span data-stu-id="fcf31-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="fcf31-109">Ďalšie informácie o vytváraní politík, zmenách a priraďovaní používateľov k politike nájdete v téme Správa [politík schôdzí v Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="fcf31-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="fcf31-110">Ak chcete vykonávať zmeny politiky pomocou rutín typu cmdlet prostredia PowerShell, pozrite si [časť Prehľad prostredia PowerShell služby Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="fcf31-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="fcf31-111">Pre politiky schôdzí v [Teams je potrebné použiť modul Skype for Business PowerShell.](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)</span><span class="sxs-lookup"><span data-stu-id="fcf31-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="fcf31-112">Ďalšie informácie [nájdete v dokumentácii rutiny typu cmdlet \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="fcf31-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

