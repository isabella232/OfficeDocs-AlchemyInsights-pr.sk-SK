---
title: Oprava aplikácií Microsoft 365 Ľutujeme, zobrazuje sa hlásenie o problémoch s dočasným serverom
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835286"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava hlásenia o aplikáciách služby Microsoft 365 "Ľutujeme, máme dočasné problémy so serverom"

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k aplikáciám služby Microsoft 365. Pozrite [si časť URL adresy a rozsahy IP adries.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Prejdite do **ponuky**  >  **Spustiť spustenie** a zadajte reťazec **services.msc.** Skontrolujte, či sú spustené všetky tieto služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba so zoznamom sietí
    - Informovanosť o sieťovom umiestnení
    - Denník udalostí systému Windows

Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s zvýšenými povoleniami:

**sfc /scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Chyba skúste to znova neskôr" pri aktivácii](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).