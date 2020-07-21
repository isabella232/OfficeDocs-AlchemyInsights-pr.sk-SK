---
title: Používateľovi sa zobrazí chyba AADSTS7000112 Sieť Yammer je vypnutá
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198372"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Používateľovi sa zobrazí chyba AADSTS7000112 Sieť Yammer je vypnutá

Ak sa zobrazí chyba "AADSTS7000112: aplikácia "00000005-0000-0ff1-ce00-0000000000000" (Yammer) je vypnutá", existuje problém s hlavné služby azure AD. Správca mohol vypnúť hlavný server služby blokovať prístup k sieti Yammer.

Vypnutie hlavného nastavenia služby sa neodporúča a môže spôsobiť ďalšie problémy. Ďalšie informácie o podporovanom prístupe k zablokovaniu prístupu používateľov k yammeru nájdete v téme [Vypnutie prístupu na Yammer pre používateľov služby Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Ak chcete odstrániť tento problém v Azure portál a obnoviť prístup používateľov k sieti Yammer:

1.  Otvorte stránku Azure Active Directory a vyberte **Podnikové aplikácie** podľa **Spravovať** na ľavej navigačnej table.
3.  Do vyhľadávacieho poľa zadajte výraz **Office 365 Yammer** a výberom názvu aplikácie otvorte nastavenia.
4.  Na ľavej navigačnej table vyberte položku **Vlastnosti** v časti **Spravovať.**
5.  Nastavte hodnotu Povolené pre používateľov na **Yes** **prihlásenie?** **Save**
6.  Znova sa prihláste do Yammera. Možno budete musieť vymazať súbory cookie.

Prípadne spustite príkazy prostredia PowerShell nastaviť hodnotu. Ďalšie informácie nájdete v časti ["Ľutujeme, ale máme problémy s prihlásením" chyba pri kliknutí na dlaždicu Yammer v službách Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 