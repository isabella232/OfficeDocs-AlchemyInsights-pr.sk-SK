---
title: Aktivácia problém-sme schopní sa pripojiť práve teraz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628257"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Oprava aplikácie balíka Office "sme schopní pripojiť práve teraz" správa

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:

1. Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office. Pozrite si [Office 365 adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite na **Štart** > **Spustiť**, a potom zadajte **Services. msc**. Uistite sa, že sú spustené nasledujúce služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba sieťového zoznamu
    - Povedomie o umiestnení v sieti
    - Denník udalostí systému Windows

Ak jedna z týchto služieb nie je spustená, pokúste sa ho spustiť. Ak máte problém so spustením služby, spustite nasledovný príkaz otvorením príkazového riadka so zvýšenými povoleniami:

**sfc/scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr "chyba pri aktivácii balíka Office z balíka Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).