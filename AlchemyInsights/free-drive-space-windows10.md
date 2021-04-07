---
title: Uvoľnenie miesta na disku vo Windowse 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505371"
---
# <a name="free-up-drive-space-in-windows-10"></a>Uvoľnenie miesta na disku vo Windowse 10

Existujú dve možnosti, ako vo Windowse uvoľniť miesto na disku:

- Uvoľnite miesto na disku vo Windowse 10.
- Uvoľnite miesto pre aktualizácie Windowsu 10 v externom ukladacom zariadení.

Ak máte po použití nástroja Čistenie disku stále málo miesta na disku, je možné, že sa priečinok Temp rýchlo zapĺňa súbormi aplikácií (.appx), ktoré používa Microsoft Store. Na odstránenie tohto problému resetujte Microsoft Store, vymažte vyrovnávaciu pamäť Microsoft Storeu a spustite nástroj na riešenie problémov pre Windows Update. Skôr než budete pokračovať podľa týchto krokov, skontrolujte, či je Microsoft Store zatvorený.

**1. krok: Resetovanie Microsoft Storeu**

**Poznámka** Týmto sa natrvalo odstránia údaje aplikácie v zariadení vrátane vašich predvolieb a podrobností o prihlásení.

1. Vyberte možnosti **Štart** > **Nastavenia** > **Aplikácie** > **Aplikácie a funkcie**.

1. V zozname aplikácií vyhľadajte a vyberte položku Microsoft Store.

1. Vyberte položku **Rozšírené možnosti**.

1. Posuňte sa nadol a vyberte možnosť **Resetovať** a potom **Potvrdiť resetovanie**.

**2. krok: Vymazanie vyrovnávacej pamäte Microsoft Storeu**

1. Stlačte kláves s logom Windows + R a otvorte dialógové okno Spustenie.

1. Napíšte wsreset.exe a vyberte **OK**.

1. Otvorí sa prázdne okno príkazového riadka. Približne po 10 sekundách sa okno zavrie a Microsoft Store sa automaticky otvorí.

**3. krok: Resetovanie lokality Windows Update**

1. Vyberte možnosti **Štart** > **Nastavenia** > **Aktualizácia a zabezpečenie** > **Riešenie problémov**.

1. Posuňte sa nadol a vyberte zo zoznamu položku **Windows Update** a potom možnosť **Spustiť riešenie problémov**.

1. Reštartujte počítač a skontrolujte, či problém stále pretrváva.

