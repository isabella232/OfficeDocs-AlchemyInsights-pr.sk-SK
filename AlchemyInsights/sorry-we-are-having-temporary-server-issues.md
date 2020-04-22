---
title: Oprava aplikácií balíka Office Ospravedlňujeme sa, máme dočasný server problémy správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764132"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Upevnenie aplikácie balíka Office "Ospravedlňujeme sa, máme dočasný server problémy" správa

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:

1. Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office. Pozrite si [adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite na **Štart** > **Spustiť**, a potom zadajte **Services. msc**. Uistite sa, že sú spustené nasledujúce služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba sieťového zoznamu
    - Povedomie o umiestnení v sieti
    - Denník udalostí systému Windows

Ak jedna z týchto služieb nie je spustená, pokúste sa ho spustiť. Ak máte problém so spustením služby, spustite nasledovný príkaz otvorením príkazového riadka so zvýšenými povoleniami:

**sfc/scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Prosím, skúste to znova neskôr "chyba pri aktivácii](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).