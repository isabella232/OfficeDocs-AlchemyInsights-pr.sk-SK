---
title: AntiSpam 5.4.1 DBEB catch-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717376"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f74d2-102">Riešenie problémov s doručovaním s kódom chyby 550 5.4.1 Relay Access bol odmietnutý</span><span class="sxs-lookup"><span data-stu-id="f74d2-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f74d2-103">Tento problém sa vyskytuje pri [kontrole a zistite, či je e-mailová adresa platná na zabránenie bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri zadávaní do siete Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f74d2-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="f74d2-104">Vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="f74d2-104">Try the following:</span></span>

1. <span data-ttu-id="f74d2-105">Zistite, či je problém špecifický pre celú doménu alebo jednu e-mailovú adresu:</span><span class="sxs-lookup"><span data-stu-id="f74d2-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f74d2-106">Celá doména: niekedy je potrebné synchronizovať doménu. Skúste [nastaviť doménu na interné a potom späť na autoritatívne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="f74d2-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f74d2-107">Jedna e-mailová adresa: niekedy musí byť adresa synchronizovaná. Zmena adresy servera SMTP proxy a následná zmena jej vrátenia môže pomôcť.</span><span class="sxs-lookup"><span data-stu-id="f74d2-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f74d2-108">Zistite, či je problém špecifický pre skupinu alebo verejný priečinok.</span><span class="sxs-lookup"><span data-stu-id="f74d2-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f74d2-109">Pri niektorých typoch objektov je možné, že objekty budú musieť byť manuálne vytvorené v službe Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f74d2-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f74d2-110">Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý odosielate), aby sme vám mohli pomôcť lepšie.</span><span class="sxs-lookup"><span data-stu-id="f74d2-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>