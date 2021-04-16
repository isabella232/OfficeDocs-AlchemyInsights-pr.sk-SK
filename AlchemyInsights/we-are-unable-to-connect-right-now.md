---
title: Problém s aktiváciou – nepodarilo sa nám pripojiť
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806457"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Oprava správy o aplikáciách služby Microsoft 365 "Nepodarilo sa pripojiť"

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k aplikáciám služby Microsoft 365. Pozrite [si časť URL adresy a rozsahy IP adries od spoločnosti Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Prejdite do **ponuky**  >  **Spustiť spustenie** a zadajte reťazec **services.msc.** Skontrolujte, či sú spustené všetky tieto služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba so zoznamom sietí
    - Informovanosť o sieťovom umiestnení
    - Denník udalostí systému Windows

Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s zvýšenými povoleniami:

**sfc /scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" pri aktivácii balíka Office zo služby Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)