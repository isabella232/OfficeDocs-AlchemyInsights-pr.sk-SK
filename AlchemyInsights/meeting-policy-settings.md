---
title: Nastavenie politiky schôdzí
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376820"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e66a8-102">Správa politík schôdzí v programe Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="e66a8-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e66a8-103">Politiky schôdzí sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze, ktoré sú naplánované používateľmi vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="e66a8-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e66a8-104">Niektoré funkcie politiky schôdzí nemusia byť implementované v tíme admin Center zatiaľ (tieto sú označené "pripravujeme" v dokumentácii).</span><span class="sxs-lookup"><span data-stu-id="e66a8-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e66a8-105">V tomto prípade, alebo ak ste získali chybu ako "nemôžeme aktualizovať politiku práve teraz, ale skúste to znova neskôr" v Microsoft teams admin Center, odporúčame použiť PowerShell vytvoriť alebo upraviť tímy stretnutia politiky.</span><span class="sxs-lookup"><span data-stu-id="e66a8-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e66a8-106">Ďalšie informácie o politikách schôdzí nájdete v nasledujúcich zdrojoch informácií:</span><span class="sxs-lookup"><span data-stu-id="e66a8-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e66a8-107">Informácie o vytváraní politík, vykonaní zmien a priraďovaní používateľov k politike nájdete [v téme Spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e66a8-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e66a8-108">Ak chcete vykonať zmeny politiky pomocou rutiny cmdlet prostredia PowerShell, pozrite si [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="e66a8-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e66a8-109">Musíte použiť [Skype Business PowerShell modul](https://www.microsoft.com/download/details.aspx?id=39366) pre tímy schôdze politiky.</span><span class="sxs-lookup"><span data-stu-id="e66a8-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e66a8-110">Skontrolujte [\*-csteamsmeetingpolicy rutiny cmdlet dokumentáciu](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="e66a8-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="e66a8-111">**Poznámka:** Pre používateľov môže trvať až 24 hodín, kým sa zmeny politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="e66a8-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="e66a8-112">Pravdepodobne nebudete môcť okamžite vykonať zmeny novovytvorených politík. Počkajte 4 hodiny a pokúste sa znova upraviť novovytvorenú politiku.</span><span class="sxs-lookup"><span data-stu-id="e66a8-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="e66a8-113">Ak problémy pretrvávajú, vyskúšajte PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e66a8-113">If you're still having problems, try PowerShell.</span></span>  