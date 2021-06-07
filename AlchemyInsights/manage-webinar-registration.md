---
title: Správa registrácie webového seminára
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794148"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="06827-102">Správa registrácie webového seminára</span><span class="sxs-lookup"><span data-stu-id="06827-102">Manage webinar registration</span></span>

<span data-ttu-id="06827-103">Môžete spravovať, kto sa môže zaregistrovať Teams Webinári pomocou príkazov Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="06827-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="06827-104">Ak chcete nainštalovať Teams PowerShell, pozrite si [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="06827-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="06827-105">Predvolene je funkcia *WhoCanRegister povolená* a nastavená na možnosť **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="06827-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="06827-106">Ak chcete povoliť, aby sa ktokoľvek vrátane anonymných používateľov zaregistroval, pomocou príkazu Powershell **nastavte** politiku schôdze na možnosť Všetci:</span><span class="sxs-lookup"><span data-stu-id="06827-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="06827-107">**Poznámka:** Ak je v nastaveniach schôdze vypnuté anonymné spojenie, anonymní používatelia sa môžu pripojiť k webovým seminárom.</span><span class="sxs-lookup"><span data-stu-id="06827-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="06827-108">Ďalšie informácie a povolenie tohto nastavenia nájdete v téme [Správa nastavení schôdze v Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="06827-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="06827-109">Ak chcete vypnúť registráciu schôdze, nastavte položku *AllowMeetingRegistration na hodnotu* **False**.</span><span class="sxs-lookup"><span data-stu-id="06827-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="06827-110">Ďalšie informácie o konfigurácii toho, kto sa môže zaregistrovať pre webináry, nájdete v téme Konfigurácia, [kto sa môže zaregistrovať pre webové semináre.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="06827-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="06827-111">Ďalšie informácie o nastaveniach pre Microsoft Lists nájdete v téme [Ovládanie nastavení pre zoznamy Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="06827-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
