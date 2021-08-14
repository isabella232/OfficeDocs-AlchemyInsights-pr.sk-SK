---
title: Riešenie Teams chyby prihlásenia AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953050"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Riešenie Teams chyby prihlásenia AADSTS9000411

Pri prihlasovaní do aplikácie Microsoft Teams sa môže zobraziť chybové hlásenie: Ľutujeme, ale máme problém s prihlásením vás **v programe AADSTS9000411: Žiadosť nie je správne formátovaná. Parameter login_hint je duplicitný.**

Ak chcete tento problém vyriešiť, skontrolujte, či Microsoft Teams klienti aktualizovali. Ďalšie informácie o aktualizácii klienta nájdete v téme [Aktualizácia Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ak z nejakého dôvodu nie je možné aktualizovať klienta, zapisovanie klienta do vyrovnávacej pamäte vymaže väčšinu údajov vo vyrovnávacej pamäti. Ak však aj po prihlásení z logaff/logon stále existujú problémy, ukončite Teams a vymažte vyrovnávaciu pamäť klienta takto:
1. Zavrite okno Microsoft Teams.
2. Prejdite na lokalitu %appdata%\microsoft\teams a odstráňte všetky súbory.
3. Znova otvorte Microsoft Teams.
