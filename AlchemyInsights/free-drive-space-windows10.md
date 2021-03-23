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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037948"
---
# <a name="free-up-drive-space-in-windows-10"></a>Uvoľnenie miesta na disku vo Windowse 10

Tu sú dve možnosti, ako uvoľniť miesto na disku vo Windowse:

- Uvoľnite miesto na disku vo Windowse 10.
- Uvoľnite miesto pre aktualizácie pre Windows 10 s externým ukladacím zariadením.

Ak máte stále dostatok voľného miesta na disku po použití čistenia disku, je možné, že priečinok Temp sa rýchlo vyplní súbormi Application (. Appx), ktoré používa Microsoft Store. Ak chcete tento problém vyriešiť, obnovte ukladanie, vymažte vyrovnávaciu pamäť obchodu a potom spustite Poradcu pri riešení problémov so službou Windows Update. Pred pokračovaním v týchto krokoch Skontrolujte, či je Microsoft Obchod zavretý.

**Krok 1: Vynulovanie Microsoft obchodu**

**Poznámka:** Týmto sa natrvalo odstránia údaje aplikácie v zariadení vrátane predvolieb a podrobností o prihlasovaní.

1. Vyberte položku **Start**  >  **Settings** Apps Apps  >    >  **& funkcií**.

1. V zozname aplikácií vyhľadajte a vyberte položku Microsoft Store.

1. Vyberte položku **Rozšírené možnosti**.

1. Posuňte sa nadol a vyberte položku **obnoviť** a potom **potvrďte vynulovanie**.

**Krok 2: Vymazanie vyrovnávacej pamäte Microsoft obchodu**

1. Stlačením klávesu s logom Windows + R otvorte dialógové okno spustiť.

1. Zadajte wsreset.exe a kliknite na **tlačidlo OK**.

1. Otvorí sa prázdne okno príkazového riadka. Po približne 10 sekundách sa okno zavrie a ukladací priestor sa otvorí automaticky.

**Krok 3: Vynulovanie aktualizácie Windowsu**

1. Vyberte položku **Spustiť**  >  aktualizáciu **nastavení**  >  & riešenie problémov so **zabezpečením**  >  .

1. Posuňte sa nadol a zo zoznamu vyberte položku **Windows Update** a vyberte položku **spustiť Poradcu pri riešení problémov**.

1. Reštartujte počítač a skontrolujte, či sa problém vyskytuje aj naďalej.

