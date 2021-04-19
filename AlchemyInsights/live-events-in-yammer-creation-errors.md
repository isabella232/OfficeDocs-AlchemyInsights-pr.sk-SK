---
title: Chyby pri tvorbe živých podujatí v Yammeri
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825530"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="3be72-102">Chyby pri tvorbe živých podujatí v Yammeri</span><span class="sxs-lookup"><span data-stu-id="3be72-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="3be72-103">**Tvorba živých podujatí v Yammeri**</span><span class="sxs-lookup"><span data-stu-id="3be72-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="3be72-104">V Yammeri sa vždy zobrazuje možnosť vytvorenia živého podujatia.</span><span class="sxs-lookup"><span data-stu-id="3be72-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="3be72-105">V niektorých prípadoch používateľ nemusí spĺňať predpoklady na vytvorenie živého podujatia a pri pokuse o jeho vytvorenie sa zobrazí chyba.</span><span class="sxs-lookup"><span data-stu-id="3be72-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="3be72-106">Nižšie uvedené položky sa zaoberajú bežnými príčinami tohto problému a poskytujú koncovým používateľom spôsoby jeho odstránenia.</span><span class="sxs-lookup"><span data-stu-id="3be72-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="3be72-107">**Kto môže vytvárať živé podujatia**</span><span class="sxs-lookup"><span data-stu-id="3be72-107">**Who can create live events**</span></span>
- <span data-ttu-id="3be72-108">Licenciu na Office 365 Enterprise E1, E3 alebo E5 alebo licenciu na Office 365 A3 alebo A5.</span><span class="sxs-lookup"><span data-stu-id="3be72-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="3be72-109">Povolenie na vytváranie živých podujatí v centre spravovania pre Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3be72-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="3be72-110">Povolenie na vytváranie živých podujatí v službe Microsoft Stream (pre podujatia vytvorené pomocou externej vysielacej aplikácie alebo zariadenia).</span><span class="sxs-lookup"><span data-stu-id="3be72-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="3be72-111">Úplné členstvo v tíme v organizácii (nemôže to byť hosť alebo z inej organizácie).</span><span class="sxs-lookup"><span data-stu-id="3be72-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="3be72-112">Plánovanie súkromnej schôdze, zdieľanie obrazovky a zdieľanie IP videa zapnuté v politike tímových schôdzí.</span><span class="sxs-lookup"><span data-stu-id="3be72-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="3be72-113">**Politiky tvorby živých podujatí**</span><span class="sxs-lookup"><span data-stu-id="3be72-113">**Live event creation policies**</span></span>

<span data-ttu-id="3be72-114">Yammer dodržiava politiky živých podujatí, ktoré sú nastavené v nájomníkovi služieb Office 365 pre Stream.</span><span class="sxs-lookup"><span data-stu-id="3be72-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="3be72-115">Predvolene môže živé podujatia vytvárať každý vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="3be72-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="3be72-116">Správcovia môžu [toto nastavenie zmeniť a zabrániť tak používateľom vytvoriť živé podujatie](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="3be72-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="3be72-117">Je dôležité skontrolovať, či používatelia majú povolenia na vytváranie živých podujatí, ak sa im zobrazí chyba politiky.</span><span class="sxs-lookup"><span data-stu-id="3be72-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
