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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Riešenie problémov s doručením pre kód chyby 550 5.4.1 prístup k prenosu bol odmietnutý

Tento problém sa vyskytuje pri [kontrole či e-mailová adresa je platná na zabránenie bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri vstupe do siete Microsoft. Vyskúšajte nasledujúce kroky:

1. Určiť, či problém je špecifický pre celú doménu alebo jednu e-mailovú adresu:
    - Celá doména: niekedy je potrebné synchronizovať doménu; Skúste [Nastavenie domény na interné a potom späť na autoritatívne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: niekedy sa adresa musí synchronizovať; Zmena adresy servera proxy SMTP a jeho zmena späť môže pomôcť.
2. Určite, či je problém špecifický pre skupinu alebo verejný priečinok. Pre niektoré typy objektov, objekty možno bude potrebné manuálne vytvoriť v Azure Active Directory.

Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý odosielate), aby sme vám mohli pomôcť lepšie.