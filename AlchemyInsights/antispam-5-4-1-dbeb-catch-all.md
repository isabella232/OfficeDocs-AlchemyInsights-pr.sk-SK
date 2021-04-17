---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821462"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="e8aaa-102">Odstránenie problémov s doručovaním s kódom chyby 550 5.4.1 – odmietnutý prístup na prenos</span><span class="sxs-lookup"><span data-stu-id="e8aaa-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="e8aaa-103">Tento problém sa vyskytuje [pri kontrole, či](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-mailová adresa platná, aby sa zabránilo návratom pomocou funkcie BounceBack pri vstupe do siete spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e8aaa-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="e8aaa-104">Vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="e8aaa-104">Try the following:</span></span>

1. <span data-ttu-id="e8aaa-105">Zistite, či je problém špecifický pre celú doménu alebo jednu e-mailovú adresu:</span><span class="sxs-lookup"><span data-stu-id="e8aaa-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="e8aaa-106">Celá doména: Niekedy treba synchronizovať doménu. skúste [nastaviť doménu na možnosť Interná a potom späť na možnosť Autoritatívny](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="e8aaa-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="e8aaa-107">Jedna e-mailová adresa: Niekedy je potrebné synchronizovať adresu. Zmena adresy servera proxy SMTP a jej zmena späť môže pomôcť.</span><span class="sxs-lookup"><span data-stu-id="e8aaa-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="e8aaa-108">Zistite, či je problém špecifický pre skupinu alebo verejný priečinok.</span><span class="sxs-lookup"><span data-stu-id="e8aaa-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="e8aaa-109">Pri niektorých typoch objektov môže byť potrebné manuálne vytvoriť objekty v službe Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8aaa-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="e8aaa-110">Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý chcete odoslať), aby sme vám mohli pomôcť lepšie.</span><span class="sxs-lookup"><span data-stu-id="e8aaa-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>