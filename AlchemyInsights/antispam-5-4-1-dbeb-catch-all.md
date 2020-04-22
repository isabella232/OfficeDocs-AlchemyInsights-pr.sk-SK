---
title: AntiSpam 5.4.1 DBEB catch-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707926"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="e1ef5-102">Riešenie problémov s doručením pre kód chyby 550 5.4.1 prístup k prenosu bol odmietnutý</span><span class="sxs-lookup"><span data-stu-id="e1ef5-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="e1ef5-103">Tento problém sa vyskytuje pri [kontrole či e-mailová adresa je platná na zabránenie bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri vstupe do siete Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e1ef5-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="e1ef5-104">Vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="e1ef5-104">Try the following:</span></span>

1. <span data-ttu-id="e1ef5-105">Určiť, či problém je špecifický pre celú doménu alebo jednu e-mailovú adresu:</span><span class="sxs-lookup"><span data-stu-id="e1ef5-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="e1ef5-106">Celá doména: niekedy je potrebné synchronizovať doménu; Skúste [Nastavenie domény na interné a potom späť na autoritatívne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="e1ef5-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="e1ef5-107">Jedna e-mailová adresa: niekedy sa adresa musí synchronizovať; Zmena adresy servera proxy SMTP a jeho zmena späť môže pomôcť.</span><span class="sxs-lookup"><span data-stu-id="e1ef5-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="e1ef5-108">Určite, či je problém špecifický pre skupinu alebo verejný priečinok.</span><span class="sxs-lookup"><span data-stu-id="e1ef5-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="e1ef5-109">Pre niektoré typy objektov, objekty možno bude potrebné manuálne vytvoriť v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1ef5-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="e1ef5-110">Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý odosielate), aby sme vám mohli pomôcť lepšie.</span><span class="sxs-lookup"><span data-stu-id="e1ef5-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>