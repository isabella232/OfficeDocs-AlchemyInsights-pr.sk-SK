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
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627589"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="3fd23-102">Správa politík schôdzí v programe Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="3fd23-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="3fd23-103">Politiky schôdzí sa používajú na ovládanie funkcií, ktoré sú k dispozícii účastníkom schôdze, ktoré sú naplánované používateľmi vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="3fd23-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="3fd23-104">Niektoré funkcie politiky schôdzí nemusia byť implementované v tíme admin Center zatiaľ (tieto sú označené "pripravujeme" v dokumentácii).</span><span class="sxs-lookup"><span data-stu-id="3fd23-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="3fd23-105">V tomto prípade, alebo ak ste získali chybu ako "nemôžeme aktualizovať politiku práve teraz, ale skúste to znova neskôr" v Microsoft teams admin Center, odporúčame použiť PowerShell vytvoriť alebo upraviť tímy stretnutia politiky.</span><span class="sxs-lookup"><span data-stu-id="3fd23-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="3fd23-106">Ďalšie informácie o politikách schôdzí nájdete v nasledujúcich zdrojoch informácií:</span><span class="sxs-lookup"><span data-stu-id="3fd23-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="3fd23-107">Informácie o vytváraní politík, vykonaní zmien a priraďovaní používateľov k politike nájdete [v téme Spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="3fd23-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="3fd23-108">Ak chcete vykonať zmeny politiky pomocou rutiny cmdlet prostredia PowerShell, pozrite si [Prehľad tímov PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="3fd23-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="3fd23-109">Musíte použiť [Skype Business PowerShell modul](https://www.microsoft.com/download/details.aspx?id=39366) pre tímy schôdze politiky.</span><span class="sxs-lookup"><span data-stu-id="3fd23-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="3fd23-110">Skontrolujte [\*-csteamsmeetingpolicy rutiny cmdlet dokumentáciu](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="3fd23-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="3fd23-111">**Poznámka:** Pre používateľov môže trvať až 24 hodín, kým sa zmeny politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="3fd23-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="3fd23-112">Pravdepodobne nebudete môcť okamžite vykonať zmeny novovytvorených politík. Počkajte 4 hodiny a pokúste sa znova upraviť novovytvorenú politiku.</span><span class="sxs-lookup"><span data-stu-id="3fd23-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="3fd23-113">Ak problémy pretrvávajú, vyskúšajte PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3fd23-113">If you're still having problems, try PowerShell.</span></span>  