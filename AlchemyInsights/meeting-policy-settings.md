---
title: Nastavenie politiky schôdze
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794349"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="cbaff-102">Správa politík schôdze v aplikácii Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="cbaff-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="cbaff-103">**Poznámka: Ak chcete, aby sa zmeny politiky prejavili pre používateľov, môže trvať až 24 hodín.**</span><span class="sxs-lookup"><span data-stu-id="cbaff-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="cbaff-104">Možno nebudete môcť okamžite vykonávať zmeny v novovytvorených politikách. Počkajte 4 hodiny a pokúste sa znova upraviť novo vytvorenú politiku.</span><span class="sxs-lookup"><span data-stu-id="cbaff-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="cbaff-105">Politiky schôdze sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze pre schôdze, ktoré naplánovali používatelia vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="cbaff-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="cbaff-106">Niektoré funkcie politík schôdze sa nemusia implementovať v centre spravovania pre Teams (tieto sú označené ako čoskoro v dokumentácii).</span><span class="sxs-lookup"><span data-stu-id="cbaff-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="cbaff-107">V tomto prípade alebo ak sa zobrazuje chybové hlásenie "momentálne nemôžeme aktualizovať politiku, ale skúste to znova neskôr" v centre spravovania služieb Microsoft Teams, odporúčame použiť prostredie PowerShell na vytvorenie alebo úpravu politík schôdze v aplikácii teams.</span><span class="sxs-lookup"><span data-stu-id="cbaff-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="cbaff-108">Ďalšie informácie o politikách schôdze nájdete v týchto zdrojoch informácií:</span><span class="sxs-lookup"><span data-stu-id="cbaff-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="cbaff-109">Ďalšie informácie o vytváraní politík, vykonávaní zmien a priradení používateľov k politike nájdete [v téme Správa politík schôdze v aplikácii teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="cbaff-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="cbaff-110">Ak chcete vykonať zmeny politiky pomocou rutiny typu cmdlet prostredia PowerShell, pozrite si tému [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="cbaff-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="cbaff-111">Na politiku schôdze v aplikácii teams musíte použiť [modul PowerShell pre Skype for Business](https://www.microsoft.com/download/details.aspx?id=39366) .</span><span class="sxs-lookup"><span data-stu-id="cbaff-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="cbaff-112">Ďalšie informácie nájdete v [dokumentácii k rutine cmdlet \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="cbaff-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

