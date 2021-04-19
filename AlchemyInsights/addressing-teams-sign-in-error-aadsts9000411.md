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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Riešenie chyby prihlásenia aplikácie Teams AADSTS9000411

Pri prihlasovaní do aplikácie Microsoft Teams sa môže zobraziť chybové hlásenie: Ľutujeme, ale máme problém s prihlásením vás **v programe AADSTS9000411: Žiadosť nie je správne formátovaná. Parameter login_hint je duplicitný.**

Ak chcete vyriešiť tento problém, uistite sa, že vaši klienti Microsoft Teams sú aktualizovaní. Ďalšie informácie o aktualizácii klienta nájdete v téme [Aktualizácia aplikácie Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ak z nejakého dôvodu nie je možné aktualizovať klienta, zapisovanie klienta do vyrovnávacej pamäte vymaže väčšinu údajov vo vyrovnávacej pamäti. Ak však aj po prihlásení z logaff/logon máte problémy, zatvorte aplikáciu Teams a vymažte vyrovnávaciu pamäť klienta takto:
1. Zavrite Microsoft Teams.
2. Prejdite na lokalitu %appdata%\microsoft\teams a odstráňte všetky súbory.
3. Znova otvorte aplikáciu Microsoft Teams.
