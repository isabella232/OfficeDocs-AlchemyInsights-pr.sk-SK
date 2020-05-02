---
title: Chyby pri tvorbe živých podujatí v Yammeri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948017"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="dc296-102">Chyby pri tvorbe živých podujatí v Yammeri</span><span class="sxs-lookup"><span data-stu-id="dc296-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="dc296-103">**Tvorba živých podujatí v Yammeri**</span><span class="sxs-lookup"><span data-stu-id="dc296-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="dc296-104">V Yammeri sa vždy zobrazuje možnosť vytvorenia živého podujatia.</span><span class="sxs-lookup"><span data-stu-id="dc296-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="dc296-105">V niektorých prípadoch používateľ nemusí spĺňať predpoklady na vytvorenie živého podujatia a pri pokuse o jeho vytvorenie sa zobrazí chyba.</span><span class="sxs-lookup"><span data-stu-id="dc296-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="dc296-106">Nižšie uvedené položky sa zaoberajú bežnými príčinami tohto problému a poskytujú koncovým používateľom spôsoby jeho odstránenia.</span><span class="sxs-lookup"><span data-stu-id="dc296-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="dc296-107">**Kto môže vytvárať živé podujatia**</span><span class="sxs-lookup"><span data-stu-id="dc296-107">**Who can create live events**</span></span>
- <span data-ttu-id="dc296-108">Licenciu na Office 365 Enterprise E1, E3 alebo E5 alebo licenciu na Office 365 A3 alebo A5.</span><span class="sxs-lookup"><span data-stu-id="dc296-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="dc296-109">Povolenie na vytváranie živých podujatí v centre spravovania pre Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dc296-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="dc296-110">Povolenie na vytváranie živých podujatí v službe Microsoft Stream (pre podujatia vytvorené pomocou externej vysielacej aplikácie alebo zariadenia).</span><span class="sxs-lookup"><span data-stu-id="dc296-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="dc296-111">Úplné členstvo v tíme v organizácii (nemôže to byť hosť alebo z inej organizácie).</span><span class="sxs-lookup"><span data-stu-id="dc296-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="dc296-112">Plánovanie súkromnej schôdze, zdieľanie obrazovky a zdieľanie IP videa zapnuté v politike tímových schôdzí.</span><span class="sxs-lookup"><span data-stu-id="dc296-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="dc296-113">**Politiky tvorby živých podujatí**</span><span class="sxs-lookup"><span data-stu-id="dc296-113">**Live event creation policies**</span></span>

<span data-ttu-id="dc296-114">Yammer dodržiava politiky živých podujatí, ktoré sú nastavené v nájomníkovi služieb Office 365 pre Stream.</span><span class="sxs-lookup"><span data-stu-id="dc296-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="dc296-115">Predvolene môže živé podujatia vytvárať každý vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="dc296-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="dc296-116">Správcovia môžu [toto nastavenie zmeniť a zabrániť tak používateľom vytvoriť živé podujatie](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="dc296-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="dc296-117">Je dôležité skontrolovať, či používatelia majú povolenia na vytváranie živých podujatí, ak sa im zobrazí chyba politiky.</span><span class="sxs-lookup"><span data-stu-id="dc296-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
