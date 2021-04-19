---
title: Začíname so živými podujatiami v Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811975"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="a0dff-102">Začíname so živými podujatiami v Teams</span><span class="sxs-lookup"><span data-stu-id="a0dff-102">Getting started with Teams live events</span></span>

<span data-ttu-id="a0dff-103">Živé podujatia v Microsoft Teams sú rozšírením schôdzí cez Teams, ktoré umožňuje plánovať a vytvárať udalosti, ktoré sa streamujú veľkému online publiku.</span><span class="sxs-lookup"><span data-stu-id="a0dff-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="a0dff-104">Ak chcete vytvoriť živé podujatie, budete potrebovať nasledovné:</span><span class="sxs-lookup"><span data-stu-id="a0dff-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="a0dff-105">Najskôr potvrďte, že živé podujatia Teams sú [k dispozícii vo vašej krajine a oblasti](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability). Živé podujatia zatiaľ nie sú v niektorých krajinách podporované.</span><span class="sxs-lookup"><span data-stu-id="a0dff-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="a0dff-106">Ak ste priradili licencie a nastavili politiky, ale stále nie je možné vytvoriť živé podujatie Teams, je pravdepodobné, že sa nachádzate v krajine alebo oblasti, kde živé podujatia ešte nie sú k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="a0dff-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="a0dff-107">[Licenciu na Office 365 Enterprise E1, E3 alebo E5 alebo licenciu na Office 365 A3 alebo A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="a0dff-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="a0dff-108">**Poznámka**: V dôsledku nedávneho nárastu využívania aplikácie Teams sa môže stať, že keď používateľovi priradíte licenciu na Teams, úplné nastavenie môže trvať až 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="a0dff-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="a0dff-109">Dovtedy im nebudete môcť priradiť politiky Teams a nemusia mať prístup k niektorým funkciám aplikácie Teams, ako sú napríklad hovory a zvukové konferencie.</span><span class="sxs-lookup"><span data-stu-id="a0dff-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="a0dff-110">Povolenie na [vytváranie živých podujatí v centre spravovania pre Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="a0dff-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="a0dff-111">Povolenie na [vytváranie živých podujatí v službe Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (pre podujatia vytvorené pomocou externej vysielacej aplikácie alebo zariadenia).</span><span class="sxs-lookup"><span data-stu-id="a0dff-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="a0dff-112">Úplné členstvo v tíme v organizácii (nemôže to byť hosť alebo z inej organizácie).</span><span class="sxs-lookup"><span data-stu-id="a0dff-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="a0dff-113">Plánovanie súkromnej schôdze, zdieľanie obrazovky a zdieľanie IP videa zapnuté v politike tímových schôdzí.</span><span class="sxs-lookup"><span data-stu-id="a0dff-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="a0dff-114">[Osvedčené postupy](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) pre živé udalosti v Teams.</span><span class="sxs-lookup"><span data-stu-id="a0dff-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="a0dff-115">Ďalšie informácie nájdete v článku [Začíname so živými podujatiami v Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="a0dff-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>