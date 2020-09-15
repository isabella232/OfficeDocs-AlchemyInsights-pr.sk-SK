---
title: AntiSpam 5.4.1 DBEB catch-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717376"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Riešenie problémov s doručovaním s kódom chyby 550 5.4.1 Relay Access bol odmietnutý

Tento problém sa vyskytuje pri [kontrole a zistite, či je e-mailová adresa platná na zabránenie bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri zadávaní do siete Microsoft. Vyskúšajte tento postup:

1. Zistite, či je problém špecifický pre celú doménu alebo jednu e-mailovú adresu:
    - Celá doména: niekedy je potrebné synchronizovať doménu. Skúste [nastaviť doménu na interné a potom späť na autoritatívne](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: niekedy musí byť adresa synchronizovaná. Zmena adresy servera SMTP proxy a následná zmena jej vrátenia môže pomôcť.
2. Zistite, či je problém špecifický pre skupinu alebo verejný priečinok. Pri niektorých typoch objektov je možné, že objekty budú musieť byť manuálne vytvorené v službe Azure Active Directory.

Ak potrebujete ďalšiu pomoc, otvorte lístok technickej podpory a zadajte rozsah problému (vrátane typu objektu, ktorý odosielate), aby sme vám mohli pomôcť lepšie.