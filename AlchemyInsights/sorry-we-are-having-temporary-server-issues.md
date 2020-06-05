---
title: Oprava aplikácií Microsoft 365 Ľutujeme, máme dočasné problémy so serverom hlásenie
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582718"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava microsoft 365 aplikácie "Ľutujeme, máme dočasné problémy so serverom" hlásenie

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúci postup:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy, aby ste potvrdili, že neblokujú prístup na Internet k aplikáciám Microsoft 365. Pozrite [si adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite do ponuky **Spustiť**  >  **a**zadajte **text services.msc**. Uistite sa, že všetky nasledujúce služby sú spustené:
    - Automatické nastavenie pripojených sieťových zariadení
    - Služba zoznam siete
    - Povedomie o sieťovom umiestnení
    - Denník udalostí systému Windows

Ak nie je spustená nie ktorá z týchto služieb, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s právami správcu:

**Sfc / scannow SFC / scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" chyba pri aktivácii](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).