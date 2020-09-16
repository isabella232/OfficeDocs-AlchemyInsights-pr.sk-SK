---
title: Riešenie problémov s aplikáciou Microsoft 365 Ľutujeme, že sa vyskytuje hlásenie s dočasným serverom
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758260"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Riešenie problémov s aplikáciou Microsoft 365 Ľutujeme, že sa vyskytli problémy s dočasným serverom

Ak sa zobrazí toto hlásenie, vyskúšajte tieto kroky:

1. Skontrolujte bránu firewall, antivírusový softvér a nastavenia servera proxy a potvrďte, že neblokujú prístup na internet k aplikáciám Microsoft 365. Pozrite si tému [URL adresy a rozsahy IP adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite na **položku spustiť**  >  **Spustenie**a zadajte výraz **Services. msc**. Uistite sa, že sú spustené tieto služby:
    - Automatické nastavenie sieťových pripojení k zariadeniam
    - Služba sieťového zoznamu
    - Povedomie o sieťovom umiestnení
    - Denník udalostí systému Windows

Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s povoleniami s právami správcu:

**sfc/scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v téme [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr pri aktivácii sa zobrazí chyba](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).