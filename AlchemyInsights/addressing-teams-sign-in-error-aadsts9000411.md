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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Riešenie tímov Sign-in chyba AADSTS9000411

Pri prihlasovaní do Microsoft teams sa môže zobraziť chyba: **Ľutujeme, ale máme problémy s prihlásením sa do AADSTS9000411: požiadavka nie je správne naformátovaná. Parameter "login_hint" sa duplikuje.**

Ak chcete vyriešiť tento problém, uistite sa, že vaši klienti Microsoft teams sú aktualizované. Ďalšie informácie o aktualizácii klienta nájdete v téme [Aktualizácia tímov Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ak nie je možné aktualizovať klienta z nejakého dôvodu, odhlásenie klienta bude jasné väčšina cache údajov. Avšak, ak máte stále problémy po odhlásenie/prihlásenie, ukončite tímy a vymažte vyrovnávaciu pamäť klienta vykonaním nasledujúcich krokov:
1. Zatvorte program Microsoft teams.
2. Prejdite na:%AppData%\microsoft\teams a odstráňte všetky súbory.
3. Znova otvorte program Microsoft teams.
