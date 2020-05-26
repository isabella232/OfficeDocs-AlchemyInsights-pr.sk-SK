---
title: Riešenie tímov Sign-in chyba AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358371"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="70a9b-102">Riešenie tímov Sign-in chyba AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="70a9b-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="70a9b-103">Pri prihlasovaní do Microsoft teams sa môže zobraziť chyba: **Ľutujeme, ale máme problémy s prihlásením sa do AADSTS9000411: požiadavka nie je správne naformátovaná. Parameter "login_hint" sa duplikuje.**</span><span class="sxs-lookup"><span data-stu-id="70a9b-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="70a9b-104">Ak chcete vyriešiť tento problém, uistite sa, že vaši klienti Microsoft teams sú aktualizované.</span><span class="sxs-lookup"><span data-stu-id="70a9b-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="70a9b-105">Ďalšie informácie o aktualizácii klienta nájdete v téme [Aktualizácia tímov Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="70a9b-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="70a9b-106">Ak nie je možné aktualizovať klienta z nejakého dôvodu, odhlásenie klienta bude jasné väčšina cache údajov.</span><span class="sxs-lookup"><span data-stu-id="70a9b-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="70a9b-107">Avšak, ak máte stále problémy po odhlásenie/prihlásenie, ukončite tímy a vymažte vyrovnávaciu pamäť klienta vykonaním nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="70a9b-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="70a9b-108">Zatvorte program Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="70a9b-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="70a9b-109">Prejdite na:%AppData%\microsoft\teams a odstráňte všetky súbory.</span><span class="sxs-lookup"><span data-stu-id="70a9b-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="70a9b-110">Znova otvorte program Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="70a9b-110">Reopen Microsoft Teams.</span></span>
