---
title: Riešenie chyby prihlásenia aplikácie Teams AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822002"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="e177f-102">Riešenie chyby prihlásenia aplikácie Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="e177f-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="e177f-103">Pri prihlasovaní do aplikácie Microsoft Teams sa môže zobraziť chybové hlásenie: Ľutujeme, ale máme problém s prihlásením vás **v programe AADSTS9000411: Žiadosť nie je správne formátovaná. Parameter login_hint je duplicitný.**</span><span class="sxs-lookup"><span data-stu-id="e177f-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="e177f-104">Ak chcete vyriešiť tento problém, uistite sa, že vaši klienti Microsoft Teams sú aktualizovaní.</span><span class="sxs-lookup"><span data-stu-id="e177f-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="e177f-105">Ďalšie informácie o aktualizácii klienta nájdete v téme [Aktualizácia aplikácie Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="e177f-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="e177f-106">Ak z nejakého dôvodu nie je možné aktualizovať klienta, zapisovanie klienta do vyrovnávacej pamäte vymaže väčšinu údajov vo vyrovnávacej pamäti.</span><span class="sxs-lookup"><span data-stu-id="e177f-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="e177f-107">Ak však aj po prihlásení z logaff/logon máte problémy, zatvorte aplikáciu Teams a vymažte vyrovnávaciu pamäť klienta takto:</span><span class="sxs-lookup"><span data-stu-id="e177f-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="e177f-108">Zavrite Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e177f-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="e177f-109">Prejdite na lokalitu %appdata%\microsoft\teams a odstráňte všetky súbory.</span><span class="sxs-lookup"><span data-stu-id="e177f-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="e177f-110">Znova otvorte aplikáciu Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e177f-110">Reopen Microsoft Teams.</span></span>
