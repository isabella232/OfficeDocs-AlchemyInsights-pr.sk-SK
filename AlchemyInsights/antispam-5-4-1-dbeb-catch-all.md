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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964307"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Riešenie problémov s doručením pre kód chyby 550 5.4.1 prístup k prenosu bol odmietnutý

Tento problém sa vyskytuje pri [kontrole vidieť, ak e-mailová adresa je platná na zabránenie bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri vstupe do siete Office 365. Vyskúšajte nasledujúce kroky:

1. Určiť, či problém je špecifický pre celú doménu alebo jednu e-mailovú adresu:
    - Celá doména: niekedy je potrebné synchronizovať doménu; Skúste [Nastavenie domény na interné a potom späť na autoritatívne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Jedna e-mailová adresa: niekedy sa adresa musí synchronizovať; Zmena adresy servera proxy SMTP a jeho zmena späť môže pomôcť.
2. Určite, či je problém špecifický pre skupinu alebo verejný priečinok. Pre niektoré typy objektov, objekty možno bude potrebné manuálne vytvoriť v Azure Active Directory.

Ak potrebujete ďalšiu pomoc, otvorte lístok podpory a zadajte rozsah problému (includidng typ objektu, ktorý posielate), aby sme vám mohli pomôcť lepšie.