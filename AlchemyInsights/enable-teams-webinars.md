---
title: Povolenie Teams webových seminárov
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794040"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="b7f9d-102">Povolenie Teams webových seminárov</span><span class="sxs-lookup"><span data-stu-id="b7f9d-102">Enable Teams Webinars</span></span>

<span data-ttu-id="b7f9d-103">Webové semináre sú predvolene povolené.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-103">Webinars are enabled by default.</span></span> <span data-ttu-id="b7f9d-104">Pomocou príkazov prostredia PowerShell môžete spravovať, kto Teams a zaregistrovať pre Teams Teams Webinári.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="b7f9d-105">Všetci používatelia, ktorí môžu vytvoriť schôdzu, môžu tiež vytvoriť schôdzu z webového seminára.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="b7f9d-106">Ak chcete spravovať, kto môže plánovať Teams Webináre, použite *funkciu AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="b7f9d-107">Predvolene je funkcia *WhoCanRegister povolená* a nastavená na možnosť **Všetci.**</span><span class="sxs-lookup"><span data-stu-id="b7f9d-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="b7f9d-108">Ak chcete vypnúť registráciu schôdze, nastavte položku *AllowMeetingRegistration na hodnotu* **False**.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="b7f9d-109">Ak chcete tieto nastavenia zmeniť, musíte nainštalovať [Teams prostredia PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="b7f9d-110">Politiky schôdzí sa tiež vynútijú na Teams Webinári.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="b7f9d-111">Ak je napríklad v nastaveniach schôdze vypnuté anonymné spojenie, anonymní používatelia sa môžu pripojiť k webovým seminárom.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="b7f9d-112">Ďalšie informácie o konfigurácii toho, kto sa môže zaregistrovať pre webináry, nájdete v téme Konfigurácia, [kto sa môže zaregistrovať pre webové semináre.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="b7f9d-113">Ďalšie informácie o nastaveniach pre Microsoft Lists nájdete v téme [Ovládanie nastavení pre zoznamy Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>