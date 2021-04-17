---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821462"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Odstránenie problémov s doručovaním s kódom chyby 550 5.4.1 – odmietnutý prístup na prenos

Tento problém sa vyskytuje [pri kontrole, či](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-mailová adresa platná, aby sa zabránilo návratom pomocou funkcie BounceBack pri vstupe do siete spoločnosti Microsoft. Vyskúšajte tieto kroky:

1. Zistite, či je problém špecifický pre celú doménu alebo jednu e-mailovú adresu:
    - Celá doména: Niekedy treba synchronizovať doménu. skúste [nastaviť doménu na možnosť Interná a potom späť na možnosť Autoritatívny](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: Niekedy je potrebné synchronizovať adresu. Zmena adresy servera proxy SMTP a jej zmena späť môže pomôcť.
2. Zistite, či je problém špecifický pre skupinu alebo verejný priečinok. Pri niektorých typoch objektov môže byť potrebné manuálne vytvoriť objekty v službe Azure Active Directory.

Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý chcete odoslať), aby sme vám mohli pomôcť lepšie.