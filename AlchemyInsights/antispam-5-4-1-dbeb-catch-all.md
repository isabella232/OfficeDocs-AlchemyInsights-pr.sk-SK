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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932292"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Odstránenie problémov s doručovaním s kódom chyby 550 5.4.1 – odmietnutý prístup na prenos

Tento problém sa vyskytuje [pri kontrole, či](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-mailová adresa platná, aby sa zabránilo návratom pomocou funkcie BounceBack pri vstupe do siete spoločnosti Microsoft. Vyskúšajte tieto kroky:

1. Zistite, či je problém špecifický pre celú doménu alebo jednu e-mailovú adresu:
    - Celá doména: Niekedy treba synchronizovať doménu. skúste [nastaviť doménu na možnosť Interná a potom späť na možnosť Autoritatívny](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: Niekedy je potrebné synchronizovať adresu. Zmena adresy servera proxy SMTP a jej zmena späť môže pomôcť.
2. Zistite, či je problém špecifický pre skupinu alebo verejný priečinok. Pri niektorých typoch objektov môže byť potrebné manuálne vytvoriť objekty v Azure Active Directory.

Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý chcete odoslať), aby sme vám mohli pomôcť lepšie.