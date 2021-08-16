---
title: Oprava Microsoft 365 aplikácií Ľutujeme, máme problém s dočasným serverom
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
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021611"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava Microsoft 365 hlásení "Ľutujeme, máme dočasné problémy so serverom"

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet Microsoft 365 aplikáciám. Pozrite [si časť URL adresy a rozsahy IP adries.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Prejdite do **ponuky**  >  **Spustiť spustenie** a zadajte reťazec **services.msc.** Skontrolujte, či sú spustené všetky tieto služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba so zoznamom sietí
    - Informovanosť o sieťovom umiestnení
    - Windows Denník udalostí

Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s zvýšenými povoleniami:

**sfc /scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Chyba skúste to znova neskôr" pri aktivácii](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).