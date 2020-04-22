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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716187"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Oprava aplikácie balíka Office "sme schopní pripojiť práve teraz" správa

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:

1. Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office. Pozrite si [adresy URL a rozsahy adries IP spoločnosti Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite na **Štart** > **Spustiť**, a potom zadajte **Services. msc**. Uistite sa, že sú spustené nasledujúce služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba sieťového zoznamu
    - Povedomie o umiestnení v sieti
    - Denník udalostí systému Windows

Ak jedna z týchto služieb nie je spustená, pokúste sa ho spustiť. Ak máte problém so spustením služby, spustite nasledovný príkaz otvorením príkazového riadka so zvýšenými povoleniami:

**sfc/scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr "chyba pri aktivácii balíka Office od spoločnosti Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).